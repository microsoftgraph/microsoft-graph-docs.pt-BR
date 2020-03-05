---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40c3c122fe5aae65b4ed34d5178c67160a7fbe0a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525009"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="061f3-103">tipo de recurso hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="061f3-103">hardwareInformation resource type</span></span>

<span data-ttu-id="061f3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="061f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="061f3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="061f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="061f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="061f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="061f3-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="061f3-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="061f3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="061f3-108">Properties</span></span>
|<span data-ttu-id="061f3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="061f3-109">Property</span></span>|<span data-ttu-id="061f3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="061f3-110">Type</span></span>|<span data-ttu-id="061f3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="061f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="061f3-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="061f3-112">serialNumber</span></span>|<span data-ttu-id="061f3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="061f3-113">String</span></span>|<span data-ttu-id="061f3-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="061f3-114">Serial number.</span></span>|
|<span data-ttu-id="061f3-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="061f3-115">totalStorageSpace</span></span>|<span data-ttu-id="061f3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="061f3-116">Int64</span></span>|<span data-ttu-id="061f3-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="061f3-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="061f3-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="061f3-118">freeStorageSpace</span></span>|<span data-ttu-id="061f3-119">Int64</span><span class="sxs-lookup"><span data-stu-id="061f3-119">Int64</span></span>|<span data-ttu-id="061f3-120">Espaço de armazenamento livre do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="061f3-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="061f3-121">imei</span><span class="sxs-lookup"><span data-stu-id="061f3-121">imei</span></span>|<span data-ttu-id="061f3-122">String</span><span class="sxs-lookup"><span data-stu-id="061f3-122">String</span></span>|<span data-ttu-id="061f3-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="061f3-123">IMEI</span></span>|
|<span data-ttu-id="061f3-124">meid</span><span class="sxs-lookup"><span data-stu-id="061f3-124">meid</span></span>|<span data-ttu-id="061f3-125">String</span><span class="sxs-lookup"><span data-stu-id="061f3-125">String</span></span>|<span data-ttu-id="061f3-126">MEID</span><span class="sxs-lookup"><span data-stu-id="061f3-126">MEID</span></span>|
|<span data-ttu-id="061f3-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="061f3-127">manufacturer</span></span>|<span data-ttu-id="061f3-128">String</span><span class="sxs-lookup"><span data-stu-id="061f3-128">String</span></span>|<span data-ttu-id="061f3-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="061f3-130">modelo</span><span class="sxs-lookup"><span data-stu-id="061f3-130">model</span></span>|<span data-ttu-id="061f3-131">String</span><span class="sxs-lookup"><span data-stu-id="061f3-131">String</span></span>|<span data-ttu-id="061f3-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-132">Model of the device</span></span>|
|<span data-ttu-id="061f3-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="061f3-133">phoneNumber</span></span>|<span data-ttu-id="061f3-134">String</span><span class="sxs-lookup"><span data-stu-id="061f3-134">String</span></span>|<span data-ttu-id="061f3-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-135">Phone number of the device</span></span>|
|<span data-ttu-id="061f3-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="061f3-136">subscriberCarrier</span></span>|<span data-ttu-id="061f3-137">String</span><span class="sxs-lookup"><span data-stu-id="061f3-137">String</span></span>|<span data-ttu-id="061f3-138">Operadora do assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="061f3-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="061f3-139">cellularTechnology</span></span>|<span data-ttu-id="061f3-140">String</span><span class="sxs-lookup"><span data-stu-id="061f3-140">String</span></span>|<span data-ttu-id="061f3-141">Tecnologia celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="061f3-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="061f3-142">wifiMac</span></span>|<span data-ttu-id="061f3-143">String</span><span class="sxs-lookup"><span data-stu-id="061f3-143">String</span></span>|<span data-ttu-id="061f3-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="061f3-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="061f3-145">operatingSystemLanguage</span></span>|<span data-ttu-id="061f3-146">String</span><span class="sxs-lookup"><span data-stu-id="061f3-146">String</span></span>|<span data-ttu-id="061f3-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-147">Operating system language of the device</span></span>|
|<span data-ttu-id="061f3-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="061f3-148">isSupervised</span></span>|<span data-ttu-id="061f3-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="061f3-149">Boolean</span></span>|<span data-ttu-id="061f3-150">Modo supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="061f3-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="061f3-151">isEncrypted</span></span>|<span data-ttu-id="061f3-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="061f3-152">Boolean</span></span>|<span data-ttu-id="061f3-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="061f3-153">Encryption status of the device</span></span>|
|<span data-ttu-id="061f3-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="061f3-154">isSharedDevice</span></span>|<span data-ttu-id="061f3-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="061f3-155">Boolean</span></span>|<span data-ttu-id="061f3-156">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="061f3-156">Shared iPad</span></span>|
|<span data-ttu-id="061f3-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="061f3-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="061f3-158">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="061f3-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="061f3-159">Todos os usuários no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="061f3-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="061f3-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="061f3-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="061f3-161">String</span><span class="sxs-lookup"><span data-stu-id="061f3-161">String</span></span>|<span data-ttu-id="061f3-162">Cadeia de caracteres que especifica a versão da especificação.</span><span class="sxs-lookup"><span data-stu-id="061f3-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="061f3-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="061f3-163">operatingSystemEdition</span></span>|<span data-ttu-id="061f3-164">String</span><span class="sxs-lookup"><span data-stu-id="061f3-164">String</span></span>|<span data-ttu-id="061f3-165">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="061f3-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="061f3-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="061f3-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="061f3-167">String</span><span class="sxs-lookup"><span data-stu-id="061f3-167">String</span></span>|<span data-ttu-id="061f3-168">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum).</span><span class="sxs-lookup"><span data-stu-id="061f3-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="061f3-169">Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="061f3-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="061f3-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="061f3-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="061f3-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="061f3-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="061f3-172">Status do requisito de hardware de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="061f3-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="061f3-173">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="061f3-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="061f3-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="061f3-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="061f3-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="061f3-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="061f3-176">Status de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="061f3-176">Virtualization-based security status.</span></span> <span data-ttu-id="061f3-177">.</span><span class="sxs-lookup"><span data-stu-id="061f3-177">.</span></span> <span data-ttu-id="061f3-178">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="061f3-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="061f3-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="061f3-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="061f3-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="061f3-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="061f3-181">Status do LSA (autoridade do sistema local)</span><span class="sxs-lookup"><span data-stu-id="061f3-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="061f3-182">.</span><span class="sxs-lookup"><span data-stu-id="061f3-182">.</span></span> <span data-ttu-id="061f3-183">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="061f3-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="061f3-184">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="061f3-184">osBuildNumber</span></span>|<span data-ttu-id="061f3-185">String</span><span class="sxs-lookup"><span data-stu-id="061f3-185">String</span></span>|<span data-ttu-id="061f3-186">Número de compilação do sistema operacional no dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="061f3-186">Operating System Build Number on Android device</span></span>|

## <a name="relationships"></a><span data-ttu-id="061f3-187">Relações</span><span class="sxs-lookup"><span data-stu-id="061f3-187">Relationships</span></span>
<span data-ttu-id="061f3-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="061f3-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="061f3-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="061f3-189">JSON Representation</span></span>
<span data-ttu-id="061f3-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="061f3-190">Here is a JSON representation of the resource.</span></span>
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



