---
title: tipo de recurso de hardwareInformation
description: Informações de hardware de um determinado dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32b6d0e637c477265a6d23f39e531ca89c7e490c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394821"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="0d8fc-103">tipo de recurso de hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0d8fc-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="0d8fc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d8fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d8fc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d8fc-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="0d8fc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d8fc-108">Properties</span></span>
|<span data-ttu-id="0d8fc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d8fc-109">Property</span></span>|<span data-ttu-id="0d8fc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-110">Type</span></span>|<span data-ttu-id="0d8fc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d8fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d8fc-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0d8fc-112">serialNumber</span></span>|<span data-ttu-id="0d8fc-113">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-113">String</span></span>|<span data-ttu-id="0d8fc-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-114">Serial number.</span></span>|
|<span data-ttu-id="0d8fc-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="0d8fc-115">totalStorageSpace</span></span>|<span data-ttu-id="0d8fc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0d8fc-116">Int64</span></span>|<span data-ttu-id="0d8fc-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="0d8fc-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="0d8fc-118">freeStorageSpace</span></span>|<span data-ttu-id="0d8fc-119">Int64</span><span class="sxs-lookup"><span data-stu-id="0d8fc-119">Int64</span></span>|<span data-ttu-id="0d8fc-120">Espaço livre de armazenamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="0d8fc-121">imei</span><span class="sxs-lookup"><span data-stu-id="0d8fc-121">imei</span></span>|<span data-ttu-id="0d8fc-122">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-122">String</span></span>|<span data-ttu-id="0d8fc-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="0d8fc-123">IMEI</span></span>|
|<span data-ttu-id="0d8fc-124">meid</span><span class="sxs-lookup"><span data-stu-id="0d8fc-124">meid</span></span>|<span data-ttu-id="0d8fc-125">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-125">String</span></span>|<span data-ttu-id="0d8fc-126">MEID</span><span class="sxs-lookup"><span data-stu-id="0d8fc-126">MEID</span></span>|
|<span data-ttu-id="0d8fc-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="0d8fc-127">manufacturer</span></span>|<span data-ttu-id="0d8fc-128">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-128">String</span></span>|<span data-ttu-id="0d8fc-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="0d8fc-130">modelo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-130">model</span></span>|<span data-ttu-id="0d8fc-131">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-131">String</span></span>|<span data-ttu-id="0d8fc-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-132">Model of the device</span></span>|
|<span data-ttu-id="0d8fc-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0d8fc-133">phoneNumber</span></span>|<span data-ttu-id="0d8fc-134">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-134">String</span></span>|<span data-ttu-id="0d8fc-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-135">Phone number of the device</span></span>|
|<span data-ttu-id="0d8fc-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0d8fc-136">subscriberCarrier</span></span>|<span data-ttu-id="0d8fc-137">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-137">String</span></span>|<span data-ttu-id="0d8fc-138">Operadora de assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="0d8fc-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="0d8fc-139">cellularTechnology</span></span>|<span data-ttu-id="0d8fc-140">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-140">String</span></span>|<span data-ttu-id="0d8fc-141">Tecnologia de celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="0d8fc-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="0d8fc-142">wifiMac</span></span>|<span data-ttu-id="0d8fc-143">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-143">String</span></span>|<span data-ttu-id="0d8fc-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="0d8fc-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="0d8fc-145">operatingSystemLanguage</span></span>|<span data-ttu-id="0d8fc-146">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-146">String</span></span>|<span data-ttu-id="0d8fc-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-147">Operating system language of the device</span></span>|
|<span data-ttu-id="0d8fc-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0d8fc-148">isSupervised</span></span>|<span data-ttu-id="0d8fc-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d8fc-149">Boolean</span></span>|<span data-ttu-id="0d8fc-150">Supervisionadas modo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="0d8fc-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0d8fc-151">isEncrypted</span></span>|<span data-ttu-id="0d8fc-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d8fc-152">Boolean</span></span>|<span data-ttu-id="0d8fc-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d8fc-153">Encryption status of the device</span></span>|
|<span data-ttu-id="0d8fc-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="0d8fc-154">isSharedDevice</span></span>|<span data-ttu-id="0d8fc-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d8fc-155">Boolean</span></span>|<span data-ttu-id="0d8fc-156">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="0d8fc-156">Shared iPad</span></span>|
|<span data-ttu-id="0d8fc-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="0d8fc-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="0d8fc-158">coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="0d8fc-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="0d8fc-159">Todos os usuários no compartilhados dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="0d8fc-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="0d8fc-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="0d8fc-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="0d8fc-161">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-161">String</span></span>|<span data-ttu-id="0d8fc-162">Cadeia de caracteres que especifica a versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="0d8fc-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="0d8fc-163">operatingSystemEdition</span></span>|<span data-ttu-id="0d8fc-164">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-164">String</span></span>|<span data-ttu-id="0d8fc-165">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="0d8fc-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="0d8fc-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="0d8fc-167">String</span><span class="sxs-lookup"><span data-stu-id="0d8fc-167">String</span></span>|<span data-ttu-id="0d8fc-168">Retorna o nome de domínio totalmente qualificado do dispositivo (se houver).</span><span class="sxs-lookup"><span data-stu-id="0d8fc-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="0d8fc-169">Se o dispositivo não está associado ao domínio, ele retornará uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="0d8fc-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="0d8fc-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="0d8fc-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="0d8fc-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="0d8fc-172">Status de requisito de hardware de segurança baseada em virtualização.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="0d8fc-173">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="0d8fc-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="0d8fc-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="0d8fc-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="0d8fc-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="0d8fc-176">Status de segurança baseada em virtualização.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-176">Virtualization-based security status.</span></span> <span data-ttu-id="0d8fc-177">.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-177"></span></span> <span data-ttu-id="0d8fc-178">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="0d8fc-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="0d8fc-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="0d8fc-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="0d8fc-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="0d8fc-181">Status do protetor de credencial sistema autoridade (LSA) local.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="0d8fc-182">.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-182"></span></span> <span data-ttu-id="0d8fc-183">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d8fc-184">Relações</span><span class="sxs-lookup"><span data-stu-id="0d8fc-184">Relationships</span></span>
<span data-ttu-id="0d8fc-185">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d8fc-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d8fc-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d8fc-186">JSON Representation</span></span>
<span data-ttu-id="0d8fc-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d8fc-187">Here is a JSON representation of the resource.</span></span>
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




