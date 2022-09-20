# rlanta-pedcreator
Ped Creator for FiveM

- Easy Ped Creator

  	~~

    Citizen.CreateThread(function()
    local ped_hash = 368603149 -- Ped Hash
    local ped_coords = { x = 461.0902, y = -992.383, z = 24.7, h = 100.0 } -- Ped Coords
 
    RequestModel(ped_hash)
    while not HasModelLoaded(ped_hash) do
        Citizen.Wait(1)
    end
  
    ped_info = CreatePed(1, ped_hash, ped_coords.x, ped_coords.y, ped_coords.z, ped_coords.h, false, true)
    SetBlockingOfNonTemporaryEvents(ped_info, true) -- Don't Change
    SetPedDiesWhenInjured(ped_info, false) -- Can Die?
    SetPedCanPlayAmbientAnims(ped_info, true) -- Don't Change
    SetPedCanRagdollFromPlayerImpact(ped_info, false) -- Ped Fall Down
    SetEntityInvincible(ped_info, true)    -- Ped Invincible
    FreezeEntityPosition(ped_info, true) -- Don't Change
  TaskStartScenarioInPlace(ped_info, "WORLD_HUMAN_COP_IDLES", 0, true); -- Ped Anim
  end)

  	~~
