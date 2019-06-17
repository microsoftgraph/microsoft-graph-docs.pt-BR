---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cbbd95c495a970dfddbc3b6c78e5e784b43d297
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995193"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="1659e-103">tipo de recurso hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="1659e-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="1659e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1659e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1659e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1659e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1659e-106">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1659e-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="1659e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1659e-107">Properties</span></span>
|<span data-ttu-id="1659e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1659e-108">Property</span></span>|<span data-ttu-id="1659e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1659e-109">Type</span></span>|<span data-ttu-id="1659e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1659e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1659e-111">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1659e-111">serialNumber</span></span>|<span data-ttu-id="1659e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1659e-112">String</span></span>|<span data-ttu-id="1659e-113">Número de série.</span><span class="sxs-lookup"><span data-stu-id="1659e-113">Serial number.</span></span>|
|<span data-ttu-id="1659e-114">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="1659e-114">totalStorageSpace</span></span>|<span data-ttu-id="1659e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="1659e-115">Int64</span></span>|<span data-ttu-id="1659e-116">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1659e-116">Total storage space of the device.</span></span>|
|<span data-ttu-id="1659e-117">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="1659e-117">freeStorageSpace</span></span>|<span data-ttu-id="1659e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1659e-118">Int64</span></span>|<span data-ttu-id="1659e-119">Espaço de armazenamento livre do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1659e-119">Free storage space of the device.</span></span>|
|<span data-ttu-id="1659e-120">imei</span><span class="sxs-lookup"><span data-stu-id="1659e-120">imei</span></span>|<span data-ttu-id="1659e-121">String</span><span class="sxs-lookup"><span data-stu-id="1659e-121">String</span></span>|<span data-ttu-id="1659e-122">IMEI</span><span class="sxs-lookup"><span data-stu-id="1659e-122">IMEI</span></span>|
|<span data-ttu-id="1659e-123">meid</span><span class="sxs-lookup"><span data-stu-id="1659e-123">meid</span></span>|<span data-ttu-id="1659e-124">String</span><span class="sxs-lookup"><span data-stu-id="1659e-124">String</span></span>|<span data-ttu-id="1659e-125">MEID</span><span class="sxs-lookup"><span data-stu-id="1659e-125">MEID</span></span>|
|<span data-ttu-id="1659e-126">fabricante</span><span class="sxs-lookup"><span data-stu-id="1659e-126">manufacturer</span></span>|<span data-ttu-id="1659e-127">String</span><span class="sxs-lookup"><span data-stu-id="1659e-127">String</span></span>|<span data-ttu-id="1659e-128">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-128">Manufacturer of the device</span></span>|
|<span data-ttu-id="1659e-129">modelo</span><span class="sxs-lookup"><span data-stu-id="1659e-129">model</span></span>|<span data-ttu-id="1659e-130">String</span><span class="sxs-lookup"><span data-stu-id="1659e-130">String</span></span>|<span data-ttu-id="1659e-131">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-131">Model of the device</span></span>|
|<span data-ttu-id="1659e-132">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="1659e-132">phoneNumber</span></span>|<span data-ttu-id="1659e-133">String</span><span class="sxs-lookup"><span data-stu-id="1659e-133">String</span></span>|<span data-ttu-id="1659e-134">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-134">Phone number of the device</span></span>|
|<span data-ttu-id="1659e-135">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="1659e-135">subscriberCarrier</span></span>|<span data-ttu-id="1659e-136">String</span><span class="sxs-lookup"><span data-stu-id="1659e-136">String</span></span>|<span data-ttu-id="1659e-137">Operadora do assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-137">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="1659e-138">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="1659e-138">cellularTechnology</span></span>|<span data-ttu-id="1659e-139">String</span><span class="sxs-lookup"><span data-stu-id="1659e-139">String</span></span>|<span data-ttu-id="1659e-140">Tecnologia celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-140">Cellular technology of the device</span></span>|
|<span data-ttu-id="1659e-141">wifiMac</span><span class="sxs-lookup"><span data-stu-id="1659e-141">wifiMac</span></span>|<span data-ttu-id="1659e-142">String</span><span class="sxs-lookup"><span data-stu-id="1659e-142">String</span></span>|<span data-ttu-id="1659e-143">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-143">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="1659e-144">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="1659e-144">operatingSystemLanguage</span></span>|<span data-ttu-id="1659e-145">String</span><span class="sxs-lookup"><span data-stu-id="1659e-145">String</span></span>|<span data-ttu-id="1659e-146">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-146">Operating system language of the device</span></span>|
|<span data-ttu-id="1659e-147">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1659e-147">isSupervised</span></span>|<span data-ttu-id="1659e-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="1659e-148">Boolean</span></span>|<span data-ttu-id="1659e-149">Modo supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-149">Supervised mode of the device</span></span>|
|<span data-ttu-id="1659e-150">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="1659e-150">isEncrypted</span></span>|<span data-ttu-id="1659e-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="1659e-151">Boolean</span></span>|<span data-ttu-id="1659e-152">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1659e-152">Encryption status of the device</span></span>|
|<span data-ttu-id="1659e-153">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="1659e-153">isSharedDevice</span></span>|<span data-ttu-id="1659e-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="1659e-154">Boolean</span></span>|<span data-ttu-id="1659e-155">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="1659e-155">Shared iPad</span></span>|
|<span data-ttu-id="1659e-156">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="1659e-156">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="1659e-157">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="1659e-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="1659e-158">Todos os usuários no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="1659e-158">All users on the shared Apple device</span></span>|
|<span data-ttu-id="1659e-159">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="1659e-159">tpmSpecificationVersion</span></span>|<span data-ttu-id="1659e-160">String</span><span class="sxs-lookup"><span data-stu-id="1659e-160">String</span></span>|<span data-ttu-id="1659e-161">Cadeia de caracteres que especifica a versão da especificação.</span><span class="sxs-lookup"><span data-stu-id="1659e-161">String that specifies the specification version.</span></span>|
|<span data-ttu-id="1659e-162">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="1659e-162">operatingSystemEdition</span></span>|<span data-ttu-id="1659e-163">String</span><span class="sxs-lookup"><span data-stu-id="1659e-163">String</span></span>|<span data-ttu-id="1659e-164">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="1659e-164">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="1659e-165">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="1659e-165">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="1659e-166">String</span><span class="sxs-lookup"><span data-stu-id="1659e-166">String</span></span>|<span data-ttu-id="1659e-167">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum).</span><span class="sxs-lookup"><span data-stu-id="1659e-167">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="1659e-168">Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="1659e-168">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="1659e-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="1659e-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="1659e-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="1659e-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="1659e-171">Status do requisito de hardware de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="1659e-171">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="1659e-172">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="1659e-172">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="1659e-173">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="1659e-173">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="1659e-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="1659e-174">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="1659e-175">Status de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="1659e-175">Virtualization-based security status.</span></span> <span data-ttu-id="1659e-176">.</span><span class="sxs-lookup"><span data-stu-id="1659e-176"></span></span> <span data-ttu-id="1659e-177">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="1659e-177">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="1659e-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="1659e-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="1659e-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="1659e-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="1659e-180">Status do LSA (autoridade do sistema local)</span><span class="sxs-lookup"><span data-stu-id="1659e-180">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="1659e-181">.</span><span class="sxs-lookup"><span data-stu-id="1659e-181"></span></span> <span data-ttu-id="1659e-182">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="1659e-182">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1659e-183">Relações</span><span class="sxs-lookup"><span data-stu-id="1659e-183">Relationships</span></span>
<span data-ttu-id="1659e-184">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1659e-184">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1659e-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1659e-185">JSON Representation</span></span>
<span data-ttu-id="1659e-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1659e-186">Here is a JSON representation of the resource.</span></span>
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
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





