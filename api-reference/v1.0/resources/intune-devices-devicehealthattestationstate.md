---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2a4ab6f846b5172ca91f191f32392b915df116e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030804"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="5e8e9-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5e8e9-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="5e8e9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e8e9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e8e9-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5e8e9-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5e8e9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e8e9-106">Properties</span></span>
|<span data-ttu-id="5e8e9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e8e9-107">Property</span></span>|<span data-ttu-id="5e8e9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e8e9-108">Type</span></span>|<span data-ttu-id="5e8e9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e8e9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e8e9-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5e8e9-110">lastUpdateDateTime</span></span>|<span data-ttu-id="5e8e9-111">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-111">String</span></span>|<span data-ttu-id="5e8e9-112">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="5e8e9-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="5e8e9-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="5e8e9-113">contentNamespaceUrl</span></span>|<span data-ttu-id="5e8e9-114">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-114">String</span></span>|<span data-ttu-id="5e8e9-115">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="5e8e9-115">The DHA report version.</span></span> <span data-ttu-id="5e8e9-116">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="5e8e9-116">(Namespace version)</span></span>|
|<span data-ttu-id="5e8e9-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="5e8e9-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="5e8e9-118">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-118">String</span></span>|<span data-ttu-id="5e8e9-119">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="5e8e9-119">The DHA report version.</span></span> <span data-ttu-id="5e8e9-120">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="5e8e9-120">(Namespace version)</span></span>|
|<span data-ttu-id="5e8e9-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="5e8e9-121">contentVersion</span></span>|<span data-ttu-id="5e8e9-122">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-122">String</span></span>|<span data-ttu-id="5e8e9-123">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="5e8e9-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="5e8e9-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e8e9-124">issuedDateTime</span></span>|<span data-ttu-id="5e8e9-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e8e9-125">DateTimeOffset</span></span>|<span data-ttu-id="5e8e9-126">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="5e8e9-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="5e8e9-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="5e8e9-127">attestationIdentityKey</span></span>|<span data-ttu-id="5e8e9-128">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-128">String</span></span>|<span data-ttu-id="5e8e9-129">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="5e8e9-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="5e8e9-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="5e8e9-130">resetCount</span></span>|<span data-ttu-id="5e8e9-131">Int64</span><span class="sxs-lookup"><span data-stu-id="5e8e9-131">Int64</span></span>|<span data-ttu-id="5e8e9-132">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="5e8e9-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="5e8e9-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="5e8e9-133">restartCount</span></span>|<span data-ttu-id="5e8e9-134">Int64</span><span class="sxs-lookup"><span data-stu-id="5e8e9-134">Int64</span></span>|<span data-ttu-id="5e8e9-135">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="5e8e9-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="5e8e9-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="5e8e9-136">dataExcutionPolicy</span></span>|<span data-ttu-id="5e8e9-137">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-137">String</span></span>|<span data-ttu-id="5e8e9-138">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="5e8e9-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="5e8e9-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="5e8e9-139">bitLockerStatus</span></span>|<span data-ttu-id="5e8e9-140">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-140">String</span></span>|<span data-ttu-id="5e8e9-141">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="5e8e9-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="5e8e9-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="5e8e9-142">bootManagerVersion</span></span>|<span data-ttu-id="5e8e9-143">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-143">String</span></span>|<span data-ttu-id="5e8e9-144">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="5e8e9-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="5e8e9-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="5e8e9-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="5e8e9-146">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-146">String</span></span>|<span data-ttu-id="5e8e9-147">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="5e8e9-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="5e8e9-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="5e8e9-148">secureBoot</span></span>|<span data-ttu-id="5e8e9-149">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-149">String</span></span>|<span data-ttu-id="5e8e9-150">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="5e8e9-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="5e8e9-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="5e8e9-151">bootDebugging</span></span>|<span data-ttu-id="5e8e9-152">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-152">String</span></span>|<span data-ttu-id="5e8e9-153">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="5e8e9-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="5e8e9-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="5e8e9-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="5e8e9-155">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-155">String</span></span>|<span data-ttu-id="5e8e9-156">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="5e8e9-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="5e8e9-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="5e8e9-157">codeIntegrity</span></span>|<span data-ttu-id="5e8e9-158">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-158">String</span></span>| <span data-ttu-id="5e8e9-159">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="5e8e9-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="5e8e9-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="5e8e9-160">testSigning</span></span>|<span data-ttu-id="5e8e9-161">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-161">String</span></span>|<span data-ttu-id="5e8e9-162">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="5e8e9-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="5e8e9-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="5e8e9-163">safeMode</span></span>|<span data-ttu-id="5e8e9-164">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-164">String</span></span>|<span data-ttu-id="5e8e9-165">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="5e8e9-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="5e8e9-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="5e8e9-166">windowsPE</span></span>|<span data-ttu-id="5e8e9-167">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-167">String</span></span>|<span data-ttu-id="5e8e9-168">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="5e8e9-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="5e8e9-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="5e8e9-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="5e8e9-170">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-170">String</span></span>|<span data-ttu-id="5e8e9-171">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="5e8e9-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="5e8e9-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="5e8e9-172">virtualSecureMode</span></span>|<span data-ttu-id="5e8e9-173">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-173">String</span></span>|<span data-ttu-id="5e8e9-174">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="5e8e9-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="5e8e9-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5e8e9-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="5e8e9-176">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-176">String</span></span>|<span data-ttu-id="5e8e9-177">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="5e8e9-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="5e8e9-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="5e8e9-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="5e8e9-179">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-179">String</span></span>|<span data-ttu-id="5e8e9-180">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="5e8e9-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="5e8e9-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="5e8e9-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="5e8e9-182">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-182">String</span></span>|<span data-ttu-id="5e8e9-183">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="5e8e9-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="5e8e9-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="5e8e9-184">tpmVersion</span></span>|<span data-ttu-id="5e8e9-185">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-185">String</span></span>|<span data-ttu-id="5e8e9-186">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="5e8e9-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="5e8e9-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="5e8e9-187">pcr0</span></span>|<span data-ttu-id="5e8e9-188">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-188">String</span></span>|<span data-ttu-id="5e8e9-189">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="5e8e9-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="5e8e9-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="5e8e9-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="5e8e9-191">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-191">String</span></span>|<span data-ttu-id="5e8e9-192">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="5e8e9-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="5e8e9-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="5e8e9-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="5e8e9-194">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-194">String</span></span>|<span data-ttu-id="5e8e9-195">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="5e8e9-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="5e8e9-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="5e8e9-196">bootRevisionListInfo</span></span>|<span data-ttu-id="5e8e9-197">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-197">String</span></span>|<span data-ttu-id="5e8e9-198">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="5e8e9-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="5e8e9-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="5e8e9-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="5e8e9-200">String</span><span class="sxs-lookup"><span data-stu-id="5e8e9-200">String</span></span>|<span data-ttu-id="5e8e9-201">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="5e8e9-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="5e8e9-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="5e8e9-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="5e8e9-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e8e9-203">String</span></span>|<span data-ttu-id="5e8e9-204">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="5e8e9-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="5e8e9-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="5e8e9-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="5e8e9-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e8e9-206">String</span></span>|<span data-ttu-id="5e8e9-207">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e8e9-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e8e9-208">Relações</span><span class="sxs-lookup"><span data-stu-id="5e8e9-208">Relationships</span></span>
<span data-ttu-id="5e8e9-209">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e8e9-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e8e9-210">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e8e9-210">JSON Representation</span></span>
<span data-ttu-id="5e8e9-211">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e8e9-211">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```



