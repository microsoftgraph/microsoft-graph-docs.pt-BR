---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2875ea3a4f8ba7bd00b2a1095ecaf496c36e5ef6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081388"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="e2030-103">tipo de recurso hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="e2030-103">hardwareInformation resource type</span></span>

<span data-ttu-id="e2030-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2030-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2030-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2030-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2030-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2030-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2030-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2030-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e2030-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2030-108">Properties</span></span>
|<span data-ttu-id="e2030-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2030-109">Property</span></span>|<span data-ttu-id="e2030-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2030-110">Type</span></span>|<span data-ttu-id="e2030-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2030-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2030-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e2030-112">serialNumber</span></span>|<span data-ttu-id="e2030-113">String</span><span class="sxs-lookup"><span data-stu-id="e2030-113">String</span></span>|<span data-ttu-id="e2030-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="e2030-114">Serial number.</span></span>|
|<span data-ttu-id="e2030-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="e2030-115">totalStorageSpace</span></span>|<span data-ttu-id="e2030-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e2030-116">Int64</span></span>|<span data-ttu-id="e2030-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2030-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="e2030-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="e2030-118">freeStorageSpace</span></span>|<span data-ttu-id="e2030-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e2030-119">Int64</span></span>|<span data-ttu-id="e2030-120">Espaço de armazenamento livre do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2030-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="e2030-121">imei</span><span class="sxs-lookup"><span data-stu-id="e2030-121">imei</span></span>|<span data-ttu-id="e2030-122">String</span><span class="sxs-lookup"><span data-stu-id="e2030-122">String</span></span>|<span data-ttu-id="e2030-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="e2030-123">IMEI</span></span>|
|<span data-ttu-id="e2030-124">meid</span><span class="sxs-lookup"><span data-stu-id="e2030-124">meid</span></span>|<span data-ttu-id="e2030-125">String</span><span class="sxs-lookup"><span data-stu-id="e2030-125">String</span></span>|<span data-ttu-id="e2030-126">MEID</span><span class="sxs-lookup"><span data-stu-id="e2030-126">MEID</span></span>|
|<span data-ttu-id="e2030-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="e2030-127">manufacturer</span></span>|<span data-ttu-id="e2030-128">String</span><span class="sxs-lookup"><span data-stu-id="e2030-128">String</span></span>|<span data-ttu-id="e2030-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="e2030-130">modelo</span><span class="sxs-lookup"><span data-stu-id="e2030-130">model</span></span>|<span data-ttu-id="e2030-131">String</span><span class="sxs-lookup"><span data-stu-id="e2030-131">String</span></span>|<span data-ttu-id="e2030-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-132">Model of the device</span></span>|
|<span data-ttu-id="e2030-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e2030-133">phoneNumber</span></span>|<span data-ttu-id="e2030-134">String</span><span class="sxs-lookup"><span data-stu-id="e2030-134">String</span></span>|<span data-ttu-id="e2030-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-135">Phone number of the device</span></span>|
|<span data-ttu-id="e2030-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="e2030-136">subscriberCarrier</span></span>|<span data-ttu-id="e2030-137">String</span><span class="sxs-lookup"><span data-stu-id="e2030-137">String</span></span>|<span data-ttu-id="e2030-138">Operadora do assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="e2030-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="e2030-139">cellularTechnology</span></span>|<span data-ttu-id="e2030-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-140">String</span></span>|<span data-ttu-id="e2030-141">Tecnologia celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="e2030-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="e2030-142">wifiMac</span></span>|<span data-ttu-id="e2030-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-143">String</span></span>|<span data-ttu-id="e2030-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="e2030-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="e2030-145">operatingSystemLanguage</span></span>|<span data-ttu-id="e2030-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-146">String</span></span>|<span data-ttu-id="e2030-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-147">Operating system language of the device</span></span>|
|<span data-ttu-id="e2030-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="e2030-148">isSupervised</span></span>|<span data-ttu-id="e2030-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2030-149">Boolean</span></span>|<span data-ttu-id="e2030-150">Modo supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="e2030-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="e2030-151">isEncrypted</span></span>|<span data-ttu-id="e2030-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2030-152">Boolean</span></span>|<span data-ttu-id="e2030-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-153">Encryption status of the device</span></span>|
|<span data-ttu-id="e2030-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="e2030-154">batterySerialNumber</span></span>|<span data-ttu-id="e2030-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-155">String</span></span>|<span data-ttu-id="e2030-156">O número de série da bateria atual do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2030-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="e2030-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="e2030-157">batteryHealthPercentage</span></span>|<span data-ttu-id="e2030-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e2030-158">Int32</span></span>|<span data-ttu-id="e2030-159">A porcentagem de integridade da bateria atual do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2030-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="e2030-160">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="e2030-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="e2030-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="e2030-161">batteryChargeCycles</span></span>|<span data-ttu-id="e2030-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e2030-162">Int32</span></span>|<span data-ttu-id="e2030-163">O número de ciclos de carga que a bateria atual do dispositivo passou.</span><span class="sxs-lookup"><span data-stu-id="e2030-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="e2030-164">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="e2030-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="e2030-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="e2030-165">isSharedDevice</span></span>|<span data-ttu-id="e2030-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2030-166">Boolean</span></span>|<span data-ttu-id="e2030-167">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="e2030-167">Shared iPad</span></span>|
|<span data-ttu-id="e2030-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="e2030-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="e2030-169">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="e2030-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="e2030-170">Todos os usuários no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="e2030-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="e2030-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="e2030-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="e2030-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-172">String</span></span>|<span data-ttu-id="e2030-173">Cadeia de caracteres que especifica a versão da especificação.</span><span class="sxs-lookup"><span data-stu-id="e2030-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="e2030-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="e2030-174">operatingSystemEdition</span></span>|<span data-ttu-id="e2030-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-175">String</span></span>|<span data-ttu-id="e2030-176">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e2030-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="e2030-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="e2030-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="e2030-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-178">String</span></span>|<span data-ttu-id="e2030-179">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum).</span><span class="sxs-lookup"><span data-stu-id="e2030-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="e2030-180">Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="e2030-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="e2030-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="e2030-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="e2030-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="e2030-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="e2030-183">Status do requisito de hardware de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="e2030-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="e2030-184">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="e2030-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="e2030-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="e2030-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="e2030-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="e2030-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="e2030-187">Status de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="e2030-187">Virtualization-based security status.</span></span> <span data-ttu-id="e2030-188">.</span><span class="sxs-lookup"><span data-stu-id="e2030-188">.</span></span> <span data-ttu-id="e2030-189">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="e2030-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="e2030-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="e2030-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="e2030-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="e2030-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="e2030-192">Status do LSA (autoridade do sistema local)</span><span class="sxs-lookup"><span data-stu-id="e2030-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="e2030-193">.</span><span class="sxs-lookup"><span data-stu-id="e2030-193">.</span></span> <span data-ttu-id="e2030-194">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="e2030-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="e2030-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="e2030-195">osBuildNumber</span></span>|<span data-ttu-id="e2030-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2030-196">String</span></span>|<span data-ttu-id="e2030-197">Número de compilação do sistema operacional no dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="e2030-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="e2030-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="e2030-198">operatingSystemProductType</span></span>|<span data-ttu-id="e2030-199">Int32</span><span class="sxs-lookup"><span data-stu-id="e2030-199">Int32</span></span>|<span data-ttu-id="e2030-200">Int que especifica o produto do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="e2030-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="e2030-201">Mais detalhes aqui https://go.microsoft.com/fwlink/?linkid=2126950 .</span><span class="sxs-lookup"><span data-stu-id="e2030-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="e2030-202">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="e2030-202">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2030-203">Relações</span><span class="sxs-lookup"><span data-stu-id="e2030-203">Relationships</span></span>
<span data-ttu-id="e2030-204">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2030-204">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2030-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2030-205">JSON Representation</span></span>
<span data-ttu-id="e2030-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2030-206">Here is a JSON representation of the resource.</span></span>
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






