---
title: tipo de recurso de hardwareInformation
description: Informações de hardware de um determinado dispositivo.
ms.openlocfilehash: 90762426ef3d7b550b9a6fe89343e54d797b3a51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037547"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="5a2f6-103">tipo de recurso de hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="5a2f6-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="5a2f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a2f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a2f6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a2f6-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="5a2f6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a2f6-108">Properties</span></span>
|<span data-ttu-id="5a2f6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a2f6-109">Property</span></span>|<span data-ttu-id="5a2f6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-110">Type</span></span>|<span data-ttu-id="5a2f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a2f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2f6-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5a2f6-112">serialNumber</span></span>|<span data-ttu-id="5a2f6-113">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-113">String</span></span>|<span data-ttu-id="5a2f6-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-114">Serial number.</span></span>|
|<span data-ttu-id="5a2f6-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="5a2f6-115">totalStorageSpace</span></span>|<span data-ttu-id="5a2f6-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5a2f6-116">Int64</span></span>|<span data-ttu-id="5a2f6-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="5a2f6-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="5a2f6-118">freeStorageSpace</span></span>|<span data-ttu-id="5a2f6-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5a2f6-119">Int64</span></span>|<span data-ttu-id="5a2f6-120">Espaço livre de armazenamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="5a2f6-121">imei</span><span class="sxs-lookup"><span data-stu-id="5a2f6-121">imei</span></span>|<span data-ttu-id="5a2f6-122">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-122">String</span></span>|<span data-ttu-id="5a2f6-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="5a2f6-123">IMEI</span></span>|
|<span data-ttu-id="5a2f6-124">meid</span><span class="sxs-lookup"><span data-stu-id="5a2f6-124">meid</span></span>|<span data-ttu-id="5a2f6-125">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-125">String</span></span>|<span data-ttu-id="5a2f6-126">MEID</span><span class="sxs-lookup"><span data-stu-id="5a2f6-126">MEID</span></span>|
|<span data-ttu-id="5a2f6-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="5a2f6-127">manufacturer</span></span>|<span data-ttu-id="5a2f6-128">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-128">String</span></span>|<span data-ttu-id="5a2f6-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="5a2f6-130">modelo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-130">model</span></span>|<span data-ttu-id="5a2f6-131">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-131">String</span></span>|<span data-ttu-id="5a2f6-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-132">Model of the device</span></span>|
|<span data-ttu-id="5a2f6-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5a2f6-133">phoneNumber</span></span>|<span data-ttu-id="5a2f6-134">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-134">String</span></span>|<span data-ttu-id="5a2f6-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-135">Phone number of the device</span></span>|
|<span data-ttu-id="5a2f6-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="5a2f6-136">subscriberCarrier</span></span>|<span data-ttu-id="5a2f6-137">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-137">String</span></span>|<span data-ttu-id="5a2f6-138">Operadora de assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="5a2f6-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="5a2f6-139">cellularTechnology</span></span>|<span data-ttu-id="5a2f6-140">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-140">String</span></span>|<span data-ttu-id="5a2f6-141">Tecnologia de celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="5a2f6-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="5a2f6-142">wifiMac</span></span>|<span data-ttu-id="5a2f6-143">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-143">String</span></span>|<span data-ttu-id="5a2f6-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="5a2f6-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="5a2f6-145">operatingSystemLanguage</span></span>|<span data-ttu-id="5a2f6-146">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-146">String</span></span>|<span data-ttu-id="5a2f6-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-147">Operating system language of the device</span></span>|
|<span data-ttu-id="5a2f6-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5a2f6-148">isSupervised</span></span>|<span data-ttu-id="5a2f6-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a2f6-149">Boolean</span></span>|<span data-ttu-id="5a2f6-150">Supervisionadas modo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="5a2f6-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5a2f6-151">isEncrypted</span></span>|<span data-ttu-id="5a2f6-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a2f6-152">Boolean</span></span>|<span data-ttu-id="5a2f6-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a2f6-153">Encryption status of the device</span></span>|
|<span data-ttu-id="5a2f6-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="5a2f6-154">isSharedDevice</span></span>|<span data-ttu-id="5a2f6-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a2f6-155">Boolean</span></span>|<span data-ttu-id="5a2f6-156">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="5a2f6-156">Shared iPad</span></span>|
|<span data-ttu-id="5a2f6-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="5a2f6-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="5a2f6-158">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="5a2f6-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="5a2f6-159">Todos os usuários no compartilhados dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="5a2f6-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="5a2f6-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="5a2f6-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="5a2f6-161">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-161">String</span></span>|<span data-ttu-id="5a2f6-162">Cadeia de caracteres que especifica a versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="5a2f6-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="5a2f6-163">operatingSystemEdition</span></span>|<span data-ttu-id="5a2f6-164">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-164">String</span></span>|<span data-ttu-id="5a2f6-165">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="5a2f6-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="5a2f6-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="5a2f6-167">String</span><span class="sxs-lookup"><span data-stu-id="5a2f6-167">String</span></span>|<span data-ttu-id="5a2f6-168">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver).</span><span class="sxs-lookup"><span data-stu-id="5a2f6-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="5a2f6-169">Se o dispositivo não está associado ao domínio, ele retornará uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="5a2f6-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="5a2f6-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="5a2f6-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="5a2f6-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="5a2f6-172">Status de requisito de hardware de segurança baseada em virtualização.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="5a2f6-173">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="5a2f6-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="5a2f6-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="5a2f6-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="5a2f6-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="5a2f6-176">Status de segurança baseada em virtualização.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-176">Virtualization-based security status.</span></span> <span data-ttu-id="5a2f6-177">.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-177"></span></span> <span data-ttu-id="5a2f6-178">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="5a2f6-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="5a2f6-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="5a2f6-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="5a2f6-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="5a2f6-181">Status do protetor de credencial sistema autoridade (LSA) local.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="5a2f6-182">.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-182"></span></span> <span data-ttu-id="5a2f6-183">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a2f6-184">Relações</span><span class="sxs-lookup"><span data-stu-id="5a2f6-184">Relationships</span></span>
<span data-ttu-id="5a2f6-185">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a2f6-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a2f6-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a2f6-186">JSON Representation</span></span>
<span data-ttu-id="5a2f6-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a2f6-187">Here is a JSON representation of the resource.</span></span>
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





