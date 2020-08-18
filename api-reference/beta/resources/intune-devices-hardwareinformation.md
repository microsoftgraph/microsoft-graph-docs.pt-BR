---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 369631fc29203c54ef3c63c2cd32df67254c76bf
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791775"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="e688c-103">tipo de recurso hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="e688c-103">hardwareInformation resource type</span></span>

<span data-ttu-id="e688c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e688c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e688c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e688c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e688c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e688c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e688c-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e688c-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e688c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e688c-108">Properties</span></span>
|<span data-ttu-id="e688c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e688c-109">Property</span></span>|<span data-ttu-id="e688c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e688c-110">Type</span></span>|<span data-ttu-id="e688c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e688c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e688c-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e688c-112">serialNumber</span></span>|<span data-ttu-id="e688c-113">String</span><span class="sxs-lookup"><span data-stu-id="e688c-113">String</span></span>|<span data-ttu-id="e688c-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="e688c-114">Serial number.</span></span>|
|<span data-ttu-id="e688c-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="e688c-115">totalStorageSpace</span></span>|<span data-ttu-id="e688c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e688c-116">Int64</span></span>|<span data-ttu-id="e688c-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e688c-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="e688c-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="e688c-118">freeStorageSpace</span></span>|<span data-ttu-id="e688c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e688c-119">Int64</span></span>|<span data-ttu-id="e688c-120">Espaço de armazenamento livre do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e688c-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="e688c-121">imei</span><span class="sxs-lookup"><span data-stu-id="e688c-121">imei</span></span>|<span data-ttu-id="e688c-122">String</span><span class="sxs-lookup"><span data-stu-id="e688c-122">String</span></span>|<span data-ttu-id="e688c-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="e688c-123">IMEI</span></span>|
|<span data-ttu-id="e688c-124">meid</span><span class="sxs-lookup"><span data-stu-id="e688c-124">meid</span></span>|<span data-ttu-id="e688c-125">String</span><span class="sxs-lookup"><span data-stu-id="e688c-125">String</span></span>|<span data-ttu-id="e688c-126">MEID</span><span class="sxs-lookup"><span data-stu-id="e688c-126">MEID</span></span>|
|<span data-ttu-id="e688c-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="e688c-127">manufacturer</span></span>|<span data-ttu-id="e688c-128">String</span><span class="sxs-lookup"><span data-stu-id="e688c-128">String</span></span>|<span data-ttu-id="e688c-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="e688c-130">modelo</span><span class="sxs-lookup"><span data-stu-id="e688c-130">model</span></span>|<span data-ttu-id="e688c-131">String</span><span class="sxs-lookup"><span data-stu-id="e688c-131">String</span></span>|<span data-ttu-id="e688c-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-132">Model of the device</span></span>|
|<span data-ttu-id="e688c-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e688c-133">phoneNumber</span></span>|<span data-ttu-id="e688c-134">String</span><span class="sxs-lookup"><span data-stu-id="e688c-134">String</span></span>|<span data-ttu-id="e688c-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-135">Phone number of the device</span></span>|
|<span data-ttu-id="e688c-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="e688c-136">subscriberCarrier</span></span>|<span data-ttu-id="e688c-137">String</span><span class="sxs-lookup"><span data-stu-id="e688c-137">String</span></span>|<span data-ttu-id="e688c-138">Operadora do assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="e688c-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="e688c-139">cellularTechnology</span></span>|<span data-ttu-id="e688c-140">String</span><span class="sxs-lookup"><span data-stu-id="e688c-140">String</span></span>|<span data-ttu-id="e688c-141">Tecnologia celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="e688c-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="e688c-142">wifiMac</span></span>|<span data-ttu-id="e688c-143">String</span><span class="sxs-lookup"><span data-stu-id="e688c-143">String</span></span>|<span data-ttu-id="e688c-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="e688c-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="e688c-145">operatingSystemLanguage</span></span>|<span data-ttu-id="e688c-146">String</span><span class="sxs-lookup"><span data-stu-id="e688c-146">String</span></span>|<span data-ttu-id="e688c-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-147">Operating system language of the device</span></span>|
|<span data-ttu-id="e688c-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="e688c-148">isSupervised</span></span>|<span data-ttu-id="e688c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e688c-149">Boolean</span></span>|<span data-ttu-id="e688c-150">Modo supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="e688c-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="e688c-151">isEncrypted</span></span>|<span data-ttu-id="e688c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e688c-152">Boolean</span></span>|<span data-ttu-id="e688c-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-153">Encryption status of the device</span></span>|
|<span data-ttu-id="e688c-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="e688c-154">batterySerialNumber</span></span>|<span data-ttu-id="e688c-155">String</span><span class="sxs-lookup"><span data-stu-id="e688c-155">String</span></span>|<span data-ttu-id="e688c-156">O número de série da bateria atual do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e688c-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="e688c-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="e688c-157">batteryHealthPercentage</span></span>|<span data-ttu-id="e688c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e688c-158">Int32</span></span>|<span data-ttu-id="e688c-159">A porcentagem de integridade da bateria atual do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e688c-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="e688c-160">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="e688c-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="e688c-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="e688c-161">batteryChargeCycles</span></span>|<span data-ttu-id="e688c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e688c-162">Int32</span></span>|<span data-ttu-id="e688c-163">O número de ciclos de carga que a bateria atual do dispositivo passou.</span><span class="sxs-lookup"><span data-stu-id="e688c-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="e688c-164">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="e688c-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="e688c-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="e688c-165">isSharedDevice</span></span>|<span data-ttu-id="e688c-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="e688c-166">Boolean</span></span>|<span data-ttu-id="e688c-167">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="e688c-167">Shared iPad</span></span>|
|<span data-ttu-id="e688c-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="e688c-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="e688c-169">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="e688c-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="e688c-170">Todos os usuários no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="e688c-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="e688c-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="e688c-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="e688c-172">String</span><span class="sxs-lookup"><span data-stu-id="e688c-172">String</span></span>|<span data-ttu-id="e688c-173">Cadeia de caracteres que especifica a versão da especificação.</span><span class="sxs-lookup"><span data-stu-id="e688c-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="e688c-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="e688c-174">operatingSystemEdition</span></span>|<span data-ttu-id="e688c-175">String</span><span class="sxs-lookup"><span data-stu-id="e688c-175">String</span></span>|<span data-ttu-id="e688c-176">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e688c-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="e688c-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="e688c-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="e688c-178">String</span><span class="sxs-lookup"><span data-stu-id="e688c-178">String</span></span>|<span data-ttu-id="e688c-179">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum).</span><span class="sxs-lookup"><span data-stu-id="e688c-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="e688c-180">Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="e688c-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="e688c-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="e688c-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="e688c-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="e688c-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="e688c-183">Status do requisito de hardware de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="e688c-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="e688c-184">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="e688c-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="e688c-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="e688c-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="e688c-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="e688c-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="e688c-187">Status de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="e688c-187">Virtualization-based security status.</span></span> <span data-ttu-id="e688c-188">.</span><span class="sxs-lookup"><span data-stu-id="e688c-188">.</span></span> <span data-ttu-id="e688c-189">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="e688c-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="e688c-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="e688c-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="e688c-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="e688c-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="e688c-192">Status do LSA (autoridade do sistema local)</span><span class="sxs-lookup"><span data-stu-id="e688c-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="e688c-193">.</span><span class="sxs-lookup"><span data-stu-id="e688c-193">.</span></span> <span data-ttu-id="e688c-194">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="e688c-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="e688c-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="e688c-195">osBuildNumber</span></span>|<span data-ttu-id="e688c-196">String</span><span class="sxs-lookup"><span data-stu-id="e688c-196">String</span></span>|<span data-ttu-id="e688c-197">Número de compilação do sistema operacional no dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="e688c-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="e688c-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="e688c-198">operatingSystemProductType</span></span>|<span data-ttu-id="e688c-199">Int32</span><span class="sxs-lookup"><span data-stu-id="e688c-199">Int32</span></span>|<span data-ttu-id="e688c-200">Int que especifica o produto do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="e688c-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="e688c-201">Mais detalhes aqui https://go.microsoft.com/fwlink/?linkid=2126950 .</span><span class="sxs-lookup"><span data-stu-id="e688c-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="e688c-202">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="e688c-202">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="e688c-203">Relações</span><span class="sxs-lookup"><span data-stu-id="e688c-203">Relationships</span></span>
<span data-ttu-id="e688c-204">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e688c-204">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e688c-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e688c-205">JSON Representation</span></span>
<span data-ttu-id="e688c-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e688c-206">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "batterySerialNumber": "String",
  "batteryHealthPercentage": 1024,
  "batteryChargeCycles": 1024,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
  "osBuildNumber": "String",
  "operatingSystemProductType": 1024
}
```



