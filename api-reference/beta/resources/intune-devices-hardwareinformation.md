---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15369ff988d13e7d083358dceb874da2a0ffa6a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470639"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="5fc63-103">tipo de recurso hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="5fc63-103">hardwareInformation resource type</span></span>

<span data-ttu-id="5fc63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fc63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5fc63-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5fc63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fc63-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5fc63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fc63-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5fc63-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="5fc63-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fc63-108">Properties</span></span>
|<span data-ttu-id="5fc63-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fc63-109">Property</span></span>|<span data-ttu-id="5fc63-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fc63-110">Type</span></span>|<span data-ttu-id="5fc63-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fc63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fc63-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5fc63-112">serialNumber</span></span>|<span data-ttu-id="5fc63-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fc63-113">String</span></span>|<span data-ttu-id="5fc63-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="5fc63-114">Serial number.</span></span>|
|<span data-ttu-id="5fc63-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="5fc63-115">totalStorageSpace</span></span>|<span data-ttu-id="5fc63-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5fc63-116">Int64</span></span>|<span data-ttu-id="5fc63-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5fc63-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="5fc63-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="5fc63-118">freeStorageSpace</span></span>|<span data-ttu-id="5fc63-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5fc63-119">Int64</span></span>|<span data-ttu-id="5fc63-120">Espaço de armazenamento livre do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5fc63-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="5fc63-121">imei</span><span class="sxs-lookup"><span data-stu-id="5fc63-121">imei</span></span>|<span data-ttu-id="5fc63-122">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-122">String</span></span>|<span data-ttu-id="5fc63-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="5fc63-123">IMEI</span></span>|
|<span data-ttu-id="5fc63-124">meid</span><span class="sxs-lookup"><span data-stu-id="5fc63-124">meid</span></span>|<span data-ttu-id="5fc63-125">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-125">String</span></span>|<span data-ttu-id="5fc63-126">MEID</span><span class="sxs-lookup"><span data-stu-id="5fc63-126">MEID</span></span>|
|<span data-ttu-id="5fc63-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="5fc63-127">manufacturer</span></span>|<span data-ttu-id="5fc63-128">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-128">String</span></span>|<span data-ttu-id="5fc63-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="5fc63-130">modelo</span><span class="sxs-lookup"><span data-stu-id="5fc63-130">model</span></span>|<span data-ttu-id="5fc63-131">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-131">String</span></span>|<span data-ttu-id="5fc63-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-132">Model of the device</span></span>|
|<span data-ttu-id="5fc63-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5fc63-133">phoneNumber</span></span>|<span data-ttu-id="5fc63-134">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-134">String</span></span>|<span data-ttu-id="5fc63-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-135">Phone number of the device</span></span>|
|<span data-ttu-id="5fc63-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="5fc63-136">subscriberCarrier</span></span>|<span data-ttu-id="5fc63-137">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-137">String</span></span>|<span data-ttu-id="5fc63-138">Operadora do assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="5fc63-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="5fc63-139">cellularTechnology</span></span>|<span data-ttu-id="5fc63-140">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-140">String</span></span>|<span data-ttu-id="5fc63-141">Tecnologia celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="5fc63-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="5fc63-142">wifiMac</span></span>|<span data-ttu-id="5fc63-143">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-143">String</span></span>|<span data-ttu-id="5fc63-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="5fc63-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="5fc63-145">operatingSystemLanguage</span></span>|<span data-ttu-id="5fc63-146">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-146">String</span></span>|<span data-ttu-id="5fc63-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-147">Operating system language of the device</span></span>|
|<span data-ttu-id="5fc63-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5fc63-148">isSupervised</span></span>|<span data-ttu-id="5fc63-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fc63-149">Boolean</span></span>|<span data-ttu-id="5fc63-150">Modo supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="5fc63-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5fc63-151">isEncrypted</span></span>|<span data-ttu-id="5fc63-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fc63-152">Boolean</span></span>|<span data-ttu-id="5fc63-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5fc63-153">Encryption status of the device</span></span>|
|<span data-ttu-id="5fc63-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="5fc63-154">isSharedDevice</span></span>|<span data-ttu-id="5fc63-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fc63-155">Boolean</span></span>|<span data-ttu-id="5fc63-156">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="5fc63-156">Shared iPad</span></span>|
|<span data-ttu-id="5fc63-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="5fc63-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="5fc63-158">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="5fc63-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="5fc63-159">Todos os usuários no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="5fc63-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="5fc63-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="5fc63-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="5fc63-161">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-161">String</span></span>|<span data-ttu-id="5fc63-162">Cadeia de caracteres que especifica a versão da especificação.</span><span class="sxs-lookup"><span data-stu-id="5fc63-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="5fc63-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="5fc63-163">operatingSystemEdition</span></span>|<span data-ttu-id="5fc63-164">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-164">String</span></span>|<span data-ttu-id="5fc63-165">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="5fc63-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="5fc63-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="5fc63-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="5fc63-167">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-167">String</span></span>|<span data-ttu-id="5fc63-168">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum).</span><span class="sxs-lookup"><span data-stu-id="5fc63-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="5fc63-169">Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="5fc63-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="5fc63-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="5fc63-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="5fc63-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="5fc63-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="5fc63-172">Status do requisito de hardware de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="5fc63-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="5fc63-173">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="5fc63-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="5fc63-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="5fc63-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="5fc63-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="5fc63-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="5fc63-176">Status de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="5fc63-176">Virtualization-based security status.</span></span> <span data-ttu-id="5fc63-177">.</span><span class="sxs-lookup"><span data-stu-id="5fc63-177">.</span></span> <span data-ttu-id="5fc63-178">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="5fc63-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="5fc63-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="5fc63-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="5fc63-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="5fc63-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="5fc63-181">Status do LSA (autoridade do sistema local)</span><span class="sxs-lookup"><span data-stu-id="5fc63-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="5fc63-182">.</span><span class="sxs-lookup"><span data-stu-id="5fc63-182">.</span></span> <span data-ttu-id="5fc63-183">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="5fc63-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="5fc63-184">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="5fc63-184">osBuildNumber</span></span>|<span data-ttu-id="5fc63-185">String</span><span class="sxs-lookup"><span data-stu-id="5fc63-185">String</span></span>|<span data-ttu-id="5fc63-186">Número de compilação do sistema operacional no dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="5fc63-186">Operating System Build Number on Android device</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fc63-187">Relações</span><span class="sxs-lookup"><span data-stu-id="5fc63-187">Relationships</span></span>
<span data-ttu-id="5fc63-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5fc63-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fc63-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fc63-189">JSON Representation</span></span>
<span data-ttu-id="5fc63-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5fc63-190">Here is a JSON representation of the resource.</span></span>
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
  "osBuildNumber": "String"
}
```



