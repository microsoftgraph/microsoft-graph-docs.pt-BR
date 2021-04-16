---
title: Tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e17df5baad3df0237218f314cdb1c5ee99f03c6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868173"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="6d60b-103">Tipo de recurso hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="6d60b-103">hardwareInformation resource type</span></span>

<span data-ttu-id="6d60b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d60b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d60b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d60b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d60b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d60b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d60b-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d60b-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="6d60b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d60b-108">Properties</span></span>
|<span data-ttu-id="6d60b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d60b-109">Property</span></span>|<span data-ttu-id="6d60b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d60b-110">Type</span></span>|<span data-ttu-id="6d60b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d60b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d60b-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6d60b-112">serialNumber</span></span>|<span data-ttu-id="6d60b-113">String</span><span class="sxs-lookup"><span data-stu-id="6d60b-113">String</span></span>|<span data-ttu-id="6d60b-114">Número de série.</span><span class="sxs-lookup"><span data-stu-id="6d60b-114">Serial number.</span></span>|
|<span data-ttu-id="6d60b-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="6d60b-115">totalStorageSpace</span></span>|<span data-ttu-id="6d60b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6d60b-116">Int64</span></span>|<span data-ttu-id="6d60b-117">Espaço de armazenamento total do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d60b-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="6d60b-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="6d60b-118">freeStorageSpace</span></span>|<span data-ttu-id="6d60b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6d60b-119">Int64</span></span>|<span data-ttu-id="6d60b-120">Espaço de armazenamento gratuito do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d60b-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="6d60b-121">imei</span><span class="sxs-lookup"><span data-stu-id="6d60b-121">imei</span></span>|<span data-ttu-id="6d60b-122">String</span><span class="sxs-lookup"><span data-stu-id="6d60b-122">String</span></span>|<span data-ttu-id="6d60b-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="6d60b-123">IMEI</span></span>|
|<span data-ttu-id="6d60b-124">meid</span><span class="sxs-lookup"><span data-stu-id="6d60b-124">meid</span></span>|<span data-ttu-id="6d60b-125">String</span><span class="sxs-lookup"><span data-stu-id="6d60b-125">String</span></span>|<span data-ttu-id="6d60b-126">MEID</span><span class="sxs-lookup"><span data-stu-id="6d60b-126">MEID</span></span>|
|<span data-ttu-id="6d60b-127">fabricante</span><span class="sxs-lookup"><span data-stu-id="6d60b-127">manufacturer</span></span>|<span data-ttu-id="6d60b-128">String</span><span class="sxs-lookup"><span data-stu-id="6d60b-128">String</span></span>|<span data-ttu-id="6d60b-129">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="6d60b-130">modelo</span><span class="sxs-lookup"><span data-stu-id="6d60b-130">model</span></span>|<span data-ttu-id="6d60b-131">String</span><span class="sxs-lookup"><span data-stu-id="6d60b-131">String</span></span>|<span data-ttu-id="6d60b-132">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-132">Model of the device</span></span>|
|<span data-ttu-id="6d60b-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="6d60b-133">phoneNumber</span></span>|<span data-ttu-id="6d60b-134">String</span><span class="sxs-lookup"><span data-stu-id="6d60b-134">String</span></span>|<span data-ttu-id="6d60b-135">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-135">Phone number of the device</span></span>|
|<span data-ttu-id="6d60b-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="6d60b-136">subscriberCarrier</span></span>|<span data-ttu-id="6d60b-137">String</span><span class="sxs-lookup"><span data-stu-id="6d60b-137">String</span></span>|<span data-ttu-id="6d60b-138">Operadora de assinante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="6d60b-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="6d60b-139">cellularTechnology</span></span>|<span data-ttu-id="6d60b-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-140">String</span></span>|<span data-ttu-id="6d60b-141">Tecnologia celular do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="6d60b-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="6d60b-142">wifiMac</span></span>|<span data-ttu-id="6d60b-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-143">String</span></span>|<span data-ttu-id="6d60b-144">Endereço MAC WiFi do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="6d60b-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="6d60b-145">operatingSystemLanguage</span></span>|<span data-ttu-id="6d60b-146">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-146">String</span></span>|<span data-ttu-id="6d60b-147">Idioma do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-147">Operating system language of the device</span></span>|
|<span data-ttu-id="6d60b-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="6d60b-148">isSupervised</span></span>|<span data-ttu-id="6d60b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d60b-149">Boolean</span></span>|<span data-ttu-id="6d60b-150">Modo supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="6d60b-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="6d60b-151">isEncrypted</span></span>|<span data-ttu-id="6d60b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d60b-152">Boolean</span></span>|<span data-ttu-id="6d60b-153">Status de criptografia do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-153">Encryption status of the device</span></span>|
|<span data-ttu-id="6d60b-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="6d60b-154">batterySerialNumber</span></span>|<span data-ttu-id="6d60b-155">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-155">String</span></span>|<span data-ttu-id="6d60b-156">O número de série da bateria atual do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d60b-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="6d60b-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="6d60b-157">batteryHealthPercentage</span></span>|<span data-ttu-id="6d60b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6d60b-158">Int32</span></span>|<span data-ttu-id="6d60b-159">A porcentagem de saúde da bateria atual do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d60b-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="6d60b-160">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="6d60b-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="6d60b-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="6d60b-161">batteryChargeCycles</span></span>|<span data-ttu-id="6d60b-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6d60b-162">Int32</span></span>|<span data-ttu-id="6d60b-163">O número de ciclos de carga que a bateria atual do dispositivo passou.</span><span class="sxs-lookup"><span data-stu-id="6d60b-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="6d60b-164">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="6d60b-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="6d60b-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="6d60b-165">isSharedDevice</span></span>|<span data-ttu-id="6d60b-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d60b-166">Boolean</span></span>|<span data-ttu-id="6d60b-167">IPad compartilhado</span><span class="sxs-lookup"><span data-stu-id="6d60b-167">Shared iPad</span></span>|
|<span data-ttu-id="6d60b-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="6d60b-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="6d60b-169">[Coleção sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="6d60b-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="6d60b-170">Todos os usuários no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="6d60b-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="6d60b-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="6d60b-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="6d60b-172">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-172">String</span></span>|<span data-ttu-id="6d60b-173">Cadeia de caracteres que especifica a versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="6d60b-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="6d60b-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="6d60b-174">operatingSystemEdition</span></span>|<span data-ttu-id="6d60b-175">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-175">String</span></span>|<span data-ttu-id="6d60b-176">Cadeia de caracteres que especifica a edição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="6d60b-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="6d60b-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="6d60b-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="6d60b-178">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-178">String</span></span>|<span data-ttu-id="6d60b-179">Retorna o nome de domínio totalmente qualificado do dispositivo (se for o caso).</span><span class="sxs-lookup"><span data-stu-id="6d60b-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="6d60b-180">Se o dispositivo não for ingressado no domínio, ele retornará uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="6d60b-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="6d60b-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="6d60b-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="6d60b-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="6d60b-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="6d60b-183">Status do requisito de hardware de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="6d60b-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="6d60b-184">Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="6d60b-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="6d60b-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="6d60b-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="6d60b-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="6d60b-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="6d60b-187">Status de segurança baseado em virtualização.</span><span class="sxs-lookup"><span data-stu-id="6d60b-187">Virtualization-based security status.</span></span> <span data-ttu-id="6d60b-188">.</span><span class="sxs-lookup"><span data-stu-id="6d60b-188">.</span></span> <span data-ttu-id="6d60b-189">Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="6d60b-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="6d60b-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="6d60b-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="6d60b-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="6d60b-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="6d60b-192">Status do proteção de credenciais da Autoridade de Sistema Local (LSA).</span><span class="sxs-lookup"><span data-stu-id="6d60b-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="6d60b-193">.</span><span class="sxs-lookup"><span data-stu-id="6d60b-193">.</span></span> <span data-ttu-id="6d60b-194">Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="6d60b-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="6d60b-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="6d60b-195">osBuildNumber</span></span>|<span data-ttu-id="6d60b-196">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-196">String</span></span>|<span data-ttu-id="6d60b-197">Número de com build do sistema operacional no dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="6d60b-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="6d60b-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="6d60b-198">operatingSystemProductType</span></span>|<span data-ttu-id="6d60b-199">Int32</span><span class="sxs-lookup"><span data-stu-id="6d60b-199">Int32</span></span>|<span data-ttu-id="6d60b-200">Int que especifica o ProductType do Sistema Operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="6d60b-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="6d60b-201">Mais detalhes aqui https://go.microsoft.com/fwlink/?linkid=2126950 .</span><span class="sxs-lookup"><span data-stu-id="6d60b-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="6d60b-202">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="6d60b-202">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="6d60b-203">ipAddressV4</span><span class="sxs-lookup"><span data-stu-id="6d60b-203">ipAddressV4</span></span>|<span data-ttu-id="6d60b-204">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-204">String</span></span>|<span data-ttu-id="6d60b-205">IPAddressV4</span><span class="sxs-lookup"><span data-stu-id="6d60b-205">IPAddressV4</span></span>|
|<span data-ttu-id="6d60b-206">subnetAddress</span><span class="sxs-lookup"><span data-stu-id="6d60b-206">subnetAddress</span></span>|<span data-ttu-id="6d60b-207">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-207">String</span></span>|<span data-ttu-id="6d60b-208">SubnetAddress</span><span class="sxs-lookup"><span data-stu-id="6d60b-208">SubnetAddress</span></span>|
|<span data-ttu-id="6d60b-209">esimIdentifier</span><span class="sxs-lookup"><span data-stu-id="6d60b-209">esimIdentifier</span></span>|<span data-ttu-id="6d60b-210">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-210">String</span></span>|<span data-ttu-id="6d60b-211">Identificador eSIM</span><span class="sxs-lookup"><span data-stu-id="6d60b-211">eSIM identifier</span></span>|
|<span data-ttu-id="6d60b-212">systemManagementBIOSVersion</span><span class="sxs-lookup"><span data-stu-id="6d60b-212">systemManagementBIOSVersion</span></span>|<span data-ttu-id="6d60b-213">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-213">String</span></span>|<span data-ttu-id="6d60b-214">Versão do BIOS conforme relatado por SMBIOS</span><span class="sxs-lookup"><span data-stu-id="6d60b-214">BIOS version as reported by SMBIOS</span></span>|
|<span data-ttu-id="6d60b-215">tpmManufacturer</span><span class="sxs-lookup"><span data-stu-id="6d60b-215">tpmManufacturer</span></span>|<span data-ttu-id="6d60b-216">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-216">String</span></span>|<span data-ttu-id="6d60b-217">As informações de identificação que nomeia exclusivamente o fabricante do TPM</span><span class="sxs-lookup"><span data-stu-id="6d60b-217">The identifying information that uniquely names the TPM manufacturer</span></span>|
|<span data-ttu-id="6d60b-218">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="6d60b-218">tpmVersion</span></span>|<span data-ttu-id="6d60b-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d60b-219">String</span></span>|<span data-ttu-id="6d60b-220">A versão do TPM, conforme especificado pelo fabricante</span><span class="sxs-lookup"><span data-stu-id="6d60b-220">The version of the TPM, as specified by the manufacturer</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d60b-221">Relações</span><span class="sxs-lookup"><span data-stu-id="6d60b-221">Relationships</span></span>
<span data-ttu-id="6d60b-222">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d60b-222">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d60b-223">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d60b-223">JSON Representation</span></span>
<span data-ttu-id="6d60b-224">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d60b-224">Here is a JSON representation of the resource.</span></span>
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
  "subnetAddress": "String",
  "esimIdentifier": "String",
  "systemManagementBIOSVersion": "String",
  "tpmManufacturer": "String",
  "tpmVersion": "String"
}
```




