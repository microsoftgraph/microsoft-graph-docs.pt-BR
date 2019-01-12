---
title: tipo de recurso de hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0665152e3cc483f2303f458b79c891658651d91f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930310"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="83380-103">tipo de recurso de hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="83380-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="83380-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="83380-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83380-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="83380-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83380-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="83380-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83380-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83380-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="83380-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83380-108">Properties</span></span>
|<span data-ttu-id="83380-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83380-109">Property</span></span>|<span data-ttu-id="83380-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="83380-110">Type</span></span>|<span data-ttu-id="83380-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83380-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83380-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="83380-112">serialNumber</span></span>|<span data-ttu-id="83380-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-113">String</span></span>|<span data-ttu-id="83380-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="83380-114">Serial number.</span></span>|
|<span data-ttu-id="83380-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="83380-115">totalStorageSpace</span></span>|<span data-ttu-id="83380-116">Int64</span><span class="sxs-lookup"><span data-stu-id="83380-116">Int64</span></span>|<span data-ttu-id="83380-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83380-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="83380-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="83380-118">freeStorageSpace</span></span>|<span data-ttu-id="83380-119">Int64</span><span class="sxs-lookup"><span data-stu-id="83380-119">Int64</span></span>|<span data-ttu-id="83380-120">Espaço livre de armazenamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83380-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="83380-121">imei</span><span class="sxs-lookup"><span data-stu-id="83380-121">imei</span></span>|<span data-ttu-id="83380-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-122">String</span></span>|<span data-ttu-id="83380-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="83380-123">IMEI</span></span>|
|<span data-ttu-id="83380-124">meid</span><span class="sxs-lookup"><span data-stu-id="83380-124">meid</span></span>|<span data-ttu-id="83380-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-125">String</span></span>|<span data-ttu-id="83380-126">MEID</span><span class="sxs-lookup"><span data-stu-id="83380-126">MEID</span></span>|
|<span data-ttu-id="83380-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="83380-127">manufacturer</span></span>|<span data-ttu-id="83380-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-128">String</span></span>|<span data-ttu-id="83380-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="83380-130">modelo</span><span class="sxs-lookup"><span data-stu-id="83380-130">model</span></span>|<span data-ttu-id="83380-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-131">String</span></span>|<span data-ttu-id="83380-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-132">Model of the device</span></span>|
|<span data-ttu-id="83380-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="83380-133">phoneNumber</span></span>|<span data-ttu-id="83380-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-134">String</span></span>|<span data-ttu-id="83380-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-135">Phone number of the device</span></span>|
|<span data-ttu-id="83380-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="83380-136">subscriberCarrier</span></span>|<span data-ttu-id="83380-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-137">String</span></span>|<span data-ttu-id="83380-138">Operadora de assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="83380-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="83380-139">cellularTechnology</span></span>|<span data-ttu-id="83380-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-140">String</span></span>|<span data-ttu-id="83380-141">Tecnologia de celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="83380-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="83380-142">wifiMac</span></span>|<span data-ttu-id="83380-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-143">String</span></span>|<span data-ttu-id="83380-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="83380-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="83380-145">operatingSystemLanguage</span></span>|<span data-ttu-id="83380-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-146">String</span></span>|<span data-ttu-id="83380-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-147">Operating system language of the device</span></span>|
|<span data-ttu-id="83380-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="83380-148">isSupervised</span></span>|<span data-ttu-id="83380-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="83380-149">Boolean</span></span>|<span data-ttu-id="83380-150">Supervisionadas modo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="83380-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="83380-151">isEncrypted</span></span>|<span data-ttu-id="83380-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="83380-152">Boolean</span></span>|<span data-ttu-id="83380-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83380-153">Encryption status of the device</span></span>|
|<span data-ttu-id="83380-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="83380-154">isSharedDevice</span></span>|<span data-ttu-id="83380-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="83380-155">Boolean</span></span>|<span data-ttu-id="83380-156">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="83380-156">Shared iPad</span></span>|
|<span data-ttu-id="83380-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="83380-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="83380-158">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="83380-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="83380-159">Todos os usuários no compartilhados dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="83380-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="83380-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="83380-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="83380-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-161">String</span></span>|<span data-ttu-id="83380-162">Cadeia de caracteres que especifica a versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="83380-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="83380-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="83380-163">operatingSystemEdition</span></span>|<span data-ttu-id="83380-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-164">String</span></span>|<span data-ttu-id="83380-165">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="83380-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="83380-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="83380-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="83380-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83380-167">String</span></span>|<span data-ttu-id="83380-168">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver).</span><span class="sxs-lookup"><span data-stu-id="83380-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="83380-169">Se o dispositivo não está associado ao domínio, ele retornará uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="83380-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="83380-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="83380-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="83380-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="83380-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="83380-172">Status de requisito de hardware de segurança baseada em virtualização.</span><span class="sxs-lookup"><span data-stu-id="83380-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="83380-173">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="83380-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="83380-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="83380-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="83380-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="83380-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="83380-176">Status de segurança baseada em virtualização.</span><span class="sxs-lookup"><span data-stu-id="83380-176">Virtualization-based security status.</span></span> <span data-ttu-id="83380-177">.</span><span class="sxs-lookup"><span data-stu-id="83380-177"></span></span> <span data-ttu-id="83380-178">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="83380-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="83380-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="83380-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="83380-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="83380-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="83380-181">Status do protetor de credencial sistema autoridade (LSA) local.</span><span class="sxs-lookup"><span data-stu-id="83380-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="83380-182">.</span><span class="sxs-lookup"><span data-stu-id="83380-182"></span></span> <span data-ttu-id="83380-183">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="83380-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83380-184">Relações</span><span class="sxs-lookup"><span data-stu-id="83380-184">Relationships</span></span>
<span data-ttu-id="83380-185">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83380-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="83380-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83380-186">JSON Representation</span></span>
<span data-ttu-id="83380-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83380-187">Here is a JSON representation of the resource.</span></span>
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





