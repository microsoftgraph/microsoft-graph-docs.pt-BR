---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aba75cb97b15253932eda90dbd252fde640f8461
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697655"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="7f217-103">tipo de recurso hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="7f217-103">hardwareInformation resource type</span></span>

<span data-ttu-id="7f217-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f217-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f217-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f217-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f217-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f217-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f217-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f217-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="7f217-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f217-108">Properties</span></span>
|<span data-ttu-id="7f217-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f217-109">Property</span></span>|<span data-ttu-id="7f217-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f217-110">Type</span></span>|<span data-ttu-id="7f217-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f217-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f217-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7f217-112">serialNumber</span></span>|<span data-ttu-id="7f217-113">String</span><span class="sxs-lookup"><span data-stu-id="7f217-113">String</span></span>|<span data-ttu-id="7f217-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="7f217-114">Serial number.</span></span>|
|<span data-ttu-id="7f217-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="7f217-115">totalStorageSpace</span></span>|<span data-ttu-id="7f217-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7f217-116">Int64</span></span>|<span data-ttu-id="7f217-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f217-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="7f217-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="7f217-118">freeStorageSpace</span></span>|<span data-ttu-id="7f217-119">Int64</span><span class="sxs-lookup"><span data-stu-id="7f217-119">Int64</span></span>|<span data-ttu-id="7f217-120">Espaço de armazenamento livre do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f217-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="7f217-121">imei</span><span class="sxs-lookup"><span data-stu-id="7f217-121">imei</span></span>|<span data-ttu-id="7f217-122">String</span><span class="sxs-lookup"><span data-stu-id="7f217-122">String</span></span>|<span data-ttu-id="7f217-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="7f217-123">IMEI</span></span>|
|<span data-ttu-id="7f217-124">meid</span><span class="sxs-lookup"><span data-stu-id="7f217-124">meid</span></span>|<span data-ttu-id="7f217-125">String</span><span class="sxs-lookup"><span data-stu-id="7f217-125">String</span></span>|<span data-ttu-id="7f217-126">MEID</span><span class="sxs-lookup"><span data-stu-id="7f217-126">MEID</span></span>|
|<span data-ttu-id="7f217-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="7f217-127">manufacturer</span></span>|<span data-ttu-id="7f217-128">String</span><span class="sxs-lookup"><span data-stu-id="7f217-128">String</span></span>|<span data-ttu-id="7f217-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="7f217-130">modelo</span><span class="sxs-lookup"><span data-stu-id="7f217-130">model</span></span>|<span data-ttu-id="7f217-131">String</span><span class="sxs-lookup"><span data-stu-id="7f217-131">String</span></span>|<span data-ttu-id="7f217-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-132">Model of the device</span></span>|
|<span data-ttu-id="7f217-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="7f217-133">phoneNumber</span></span>|<span data-ttu-id="7f217-134">String</span><span class="sxs-lookup"><span data-stu-id="7f217-134">String</span></span>|<span data-ttu-id="7f217-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-135">Phone number of the device</span></span>|
|<span data-ttu-id="7f217-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="7f217-136">subscriberCarrier</span></span>|<span data-ttu-id="7f217-137">String</span><span class="sxs-lookup"><span data-stu-id="7f217-137">String</span></span>|<span data-ttu-id="7f217-138">Operadora do assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="7f217-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="7f217-139">cellularTechnology</span></span>|<span data-ttu-id="7f217-140">String</span><span class="sxs-lookup"><span data-stu-id="7f217-140">String</span></span>|<span data-ttu-id="7f217-141">Tecnologia celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="7f217-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="7f217-142">wifiMac</span></span>|<span data-ttu-id="7f217-143">String</span><span class="sxs-lookup"><span data-stu-id="7f217-143">String</span></span>|<span data-ttu-id="7f217-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="7f217-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="7f217-145">operatingSystemLanguage</span></span>|<span data-ttu-id="7f217-146">String</span><span class="sxs-lookup"><span data-stu-id="7f217-146">String</span></span>|<span data-ttu-id="7f217-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-147">Operating system language of the device</span></span>|
|<span data-ttu-id="7f217-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="7f217-148">isSupervised</span></span>|<span data-ttu-id="7f217-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f217-149">Boolean</span></span>|<span data-ttu-id="7f217-150">Modo supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="7f217-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="7f217-151">isEncrypted</span></span>|<span data-ttu-id="7f217-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f217-152">Boolean</span></span>|<span data-ttu-id="7f217-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-153">Encryption status of the device</span></span>|
|<span data-ttu-id="7f217-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="7f217-154">batterySerialNumber</span></span>|<span data-ttu-id="7f217-155">String</span><span class="sxs-lookup"><span data-stu-id="7f217-155">String</span></span>|<span data-ttu-id="7f217-156">O número de série da bateria atual do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f217-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="7f217-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="7f217-157">batteryHealthPercentage</span></span>|<span data-ttu-id="7f217-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7f217-158">Int32</span></span>|<span data-ttu-id="7f217-159">A porcentagem de integridade da bateria atual do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f217-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="7f217-160">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="7f217-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="7f217-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="7f217-161">batteryChargeCycles</span></span>|<span data-ttu-id="7f217-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7f217-162">Int32</span></span>|<span data-ttu-id="7f217-163">O número de ciclos de carga que a bateria atual do dispositivo passou.</span><span class="sxs-lookup"><span data-stu-id="7f217-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="7f217-164">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="7f217-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="7f217-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="7f217-165">isSharedDevice</span></span>|<span data-ttu-id="7f217-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f217-166">Boolean</span></span>|<span data-ttu-id="7f217-167">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="7f217-167">Shared iPad</span></span>|
|<span data-ttu-id="7f217-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="7f217-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="7f217-169">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="7f217-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="7f217-170">Todos os usuários no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="7f217-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="7f217-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="7f217-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="7f217-172">String</span><span class="sxs-lookup"><span data-stu-id="7f217-172">String</span></span>|<span data-ttu-id="7f217-173">Cadeia de caracteres que especifica a versão da especificação.</span><span class="sxs-lookup"><span data-stu-id="7f217-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="7f217-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="7f217-174">operatingSystemEdition</span></span>|<span data-ttu-id="7f217-175">String</span><span class="sxs-lookup"><span data-stu-id="7f217-175">String</span></span>|<span data-ttu-id="7f217-176">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="7f217-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="7f217-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="7f217-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="7f217-178">String</span><span class="sxs-lookup"><span data-stu-id="7f217-178">String</span></span>|<span data-ttu-id="7f217-179">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum).</span><span class="sxs-lookup"><span data-stu-id="7f217-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="7f217-180">Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="7f217-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="7f217-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="7f217-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="7f217-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="7f217-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="7f217-183">Status do requisito de hardware de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="7f217-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="7f217-184">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="7f217-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="7f217-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="7f217-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="7f217-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="7f217-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="7f217-187">Status de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="7f217-187">Virtualization-based security status.</span></span> <span data-ttu-id="7f217-188">.</span><span class="sxs-lookup"><span data-stu-id="7f217-188">.</span></span> <span data-ttu-id="7f217-189">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="7f217-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="7f217-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="7f217-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="7f217-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="7f217-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="7f217-192">Status do LSA (autoridade do sistema local)</span><span class="sxs-lookup"><span data-stu-id="7f217-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="7f217-193">.</span><span class="sxs-lookup"><span data-stu-id="7f217-193">.</span></span> <span data-ttu-id="7f217-194">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="7f217-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="7f217-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="7f217-195">osBuildNumber</span></span>|<span data-ttu-id="7f217-196">String</span><span class="sxs-lookup"><span data-stu-id="7f217-196">String</span></span>|<span data-ttu-id="7f217-197">Número de compilação do sistema operacional no dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="7f217-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="7f217-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="7f217-198">operatingSystemProductType</span></span>|<span data-ttu-id="7f217-199">Int32</span><span class="sxs-lookup"><span data-stu-id="7f217-199">Int32</span></span>|<span data-ttu-id="7f217-200">Int que especifica o produto do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="7f217-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="7f217-201">Mais detalhes aqui https://go.microsoft.com/fwlink/?linkid=2126950 .</span><span class="sxs-lookup"><span data-stu-id="7f217-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="7f217-202">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="7f217-202">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="7f217-203">ipAddressV4</span><span class="sxs-lookup"><span data-stu-id="7f217-203">ipAddressV4</span></span>|<span data-ttu-id="7f217-204">String</span><span class="sxs-lookup"><span data-stu-id="7f217-204">String</span></span>|<span data-ttu-id="7f217-205">IPAddressV4</span><span class="sxs-lookup"><span data-stu-id="7f217-205">IPAddressV4</span></span>|
|<span data-ttu-id="7f217-206">subnetAddress</span><span class="sxs-lookup"><span data-stu-id="7f217-206">subnetAddress</span></span>|<span data-ttu-id="7f217-207">String</span><span class="sxs-lookup"><span data-stu-id="7f217-207">String</span></span>|<span data-ttu-id="7f217-208">SubnetAddress</span><span class="sxs-lookup"><span data-stu-id="7f217-208">SubnetAddress</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f217-209">Relações</span><span class="sxs-lookup"><span data-stu-id="7f217-209">Relationships</span></span>
<span data-ttu-id="7f217-210">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f217-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f217-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f217-211">JSON Representation</span></span>
<span data-ttu-id="7f217-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f217-212">Here is a JSON representation of the resource.</span></span>
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
  "operatingSystemProductType": 1024,
  "ipAddressV4": "String",
  "subnetAddress": "String"
}
```





