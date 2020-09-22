---
title: tipo de recurso deviceHealthScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts de integridade do PowerShell (remediation + detecção) nos dispositivos do Windows 10 Azure Active Directory associados registrados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 388ac809b02316b9daf250f04fb6ce42b593a4de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060430"
---
# <a name="devicehealthscript-resource-type"></a><span data-ttu-id="23521-103">tipo de recurso deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-103">deviceHealthScript resource type</span></span>

<span data-ttu-id="23521-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23521-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23521-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23521-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23521-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23521-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23521-107">O Intune fornecerá ao cliente a capacidade de executar os scripts de integridade do PowerShell (remediation + detecção) nos dispositivos do Windows 10 Azure Active Directory associados registrados.</span><span class="sxs-lookup"><span data-stu-id="23521-107">Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.</span></span>

## <a name="methods"></a><span data-ttu-id="23521-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="23521-108">Methods</span></span>
|<span data-ttu-id="23521-109">Método</span><span class="sxs-lookup"><span data-stu-id="23521-109">Method</span></span>|<span data-ttu-id="23521-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23521-110">Return Type</span></span>|<span data-ttu-id="23521-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23521-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23521-112">Listar deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="23521-112">List deviceHealthScripts</span></span>](../api/intune-devices-devicehealthscript-list.md)|<span data-ttu-id="23521-113">coleção [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="23521-113">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md) collection</span></span>|<span data-ttu-id="23521-114">Listar Propriedades e relações dos objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="23521-114">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>|
|[<span data-ttu-id="23521-115">Obter deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-115">Get deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-get.md)|[<span data-ttu-id="23521-116">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-116">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="23521-117">Leia as propriedades e as relações do objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="23521-117">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="23521-118">Criar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-118">Create deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-create.md)|[<span data-ttu-id="23521-119">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-119">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="23521-120">Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="23521-120">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="23521-121">Excluir deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-121">Delete deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-delete.md)|<span data-ttu-id="23521-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23521-122">None</span></span>|<span data-ttu-id="23521-123">Exclui [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="23521-123">Deletes a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>|
|[<span data-ttu-id="23521-124">Atualizar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-124">Update deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-update.md)|[<span data-ttu-id="23521-125">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="23521-125">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="23521-126">Atualiza as propriedades de um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="23521-126">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="23521-127">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="23521-127">assign action</span></span>](../api/intune-devices-devicehealthscript-assign.md)|<span data-ttu-id="23521-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="23521-128">None</span></span>|<span data-ttu-id="23521-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23521-129">Not yet documented</span></span>|
|[<span data-ttu-id="23521-130">ação updateGlobalScript</span><span class="sxs-lookup"><span data-stu-id="23521-130">updateGlobalScript action</span></span>](../api/intune-devices-devicehealthscript-updateglobalscript.md)|<span data-ttu-id="23521-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23521-131">String</span></span>|<span data-ttu-id="23521-132">Atualizar o script de integridade do dispositivo proprietário</span><span class="sxs-lookup"><span data-stu-id="23521-132">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="23521-133">ação getGlobalScriptHighestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="23521-133">getGlobalScriptHighestAvailableVersion action</span></span>](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|<span data-ttu-id="23521-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23521-134">String</span></span>|<span data-ttu-id="23521-135">Atualizar o script de integridade do dispositivo proprietário</span><span class="sxs-lookup"><span data-stu-id="23521-135">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="23521-136">ação enableGlobalScripts</span><span class="sxs-lookup"><span data-stu-id="23521-136">enableGlobalScripts action</span></span>](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|<span data-ttu-id="23521-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="23521-137">None</span></span>|<span data-ttu-id="23521-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23521-138">Not yet documented</span></span>|
|[<span data-ttu-id="23521-139">função areGlobalScriptsAvailable</span><span class="sxs-lookup"><span data-stu-id="23521-139">areGlobalScriptsAvailable function</span></span>](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[<span data-ttu-id="23521-140">globalDeviceHealthScriptState</span><span class="sxs-lookup"><span data-stu-id="23521-140">globalDeviceHealthScriptState</span></span>](../resources/intune-devices-globaldevicehealthscriptstate.md)|<span data-ttu-id="23521-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23521-141">Not yet documented</span></span>|
|[<span data-ttu-id="23521-142">função getRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="23521-142">getRemediationSummary function</span></span>](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[<span data-ttu-id="23521-143">deviceHealthScriptRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="23521-143">deviceHealthScriptRemediationSummary</span></span>](../resources/intune-devices-devicehealthscriptremediationsummary.md)|<span data-ttu-id="23521-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23521-144">Not yet documented</span></span>|
|[<span data-ttu-id="23521-145">função getRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="23521-145">getRemediationHistory function</span></span>](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[<span data-ttu-id="23521-146">deviceHealthScriptRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="23521-146">deviceHealthScriptRemediationHistory</span></span>](../resources/intune-devices-devicehealthscriptremediationhistory.md)|<span data-ttu-id="23521-147">Função para obter o número de correções por scripts de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-147">Function to get the number of remediations by a device health scripts</span></span>|

## <a name="properties"></a><span data-ttu-id="23521-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23521-148">Properties</span></span>
|<span data-ttu-id="23521-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23521-149">Property</span></span>|<span data-ttu-id="23521-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="23521-150">Type</span></span>|<span data-ttu-id="23521-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="23521-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23521-152">id</span><span class="sxs-lookup"><span data-stu-id="23521-152">id</span></span>|<span data-ttu-id="23521-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23521-153">String</span></span>|<span data-ttu-id="23521-154">Identificador exclusivo do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-154">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="23521-155">publicador</span><span class="sxs-lookup"><span data-stu-id="23521-155">publisher</span></span>|<span data-ttu-id="23521-156">String</span><span class="sxs-lookup"><span data-stu-id="23521-156">String</span></span>|<span data-ttu-id="23521-157">Nome do editor de script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-157">Name of the device health script publisher</span></span>|
|<span data-ttu-id="23521-158">versão</span><span class="sxs-lookup"><span data-stu-id="23521-158">version</span></span>|<span data-ttu-id="23521-159">String</span><span class="sxs-lookup"><span data-stu-id="23521-159">String</span></span>|<span data-ttu-id="23521-160">Versão do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-160">Version of the device health script</span></span>|
|<span data-ttu-id="23521-161">displayName</span><span class="sxs-lookup"><span data-stu-id="23521-161">displayName</span></span>|<span data-ttu-id="23521-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23521-162">String</span></span>|<span data-ttu-id="23521-163">Nome do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-163">Name of the device health script</span></span>|
|<span data-ttu-id="23521-164">description</span><span class="sxs-lookup"><span data-stu-id="23521-164">description</span></span>|<span data-ttu-id="23521-165">String</span><span class="sxs-lookup"><span data-stu-id="23521-165">String</span></span>|<span data-ttu-id="23521-166">Descrição do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-166">Description of the device health script</span></span>|
|<span data-ttu-id="23521-167">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="23521-167">detectionScriptContent</span></span>|<span data-ttu-id="23521-168">Binária</span><span class="sxs-lookup"><span data-stu-id="23521-168">Binary</span></span>|<span data-ttu-id="23521-169">Todo o conteúdo do script do PowerShell de detecção</span><span class="sxs-lookup"><span data-stu-id="23521-169">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="23521-170">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="23521-170">remediationScriptContent</span></span>|<span data-ttu-id="23521-171">Binária</span><span class="sxs-lookup"><span data-stu-id="23521-171">Binary</span></span>|<span data-ttu-id="23521-172">Todo o conteúdo do script do PowerShell de correção</span><span class="sxs-lookup"><span data-stu-id="23521-172">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="23521-173">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23521-173">createdDateTime</span></span>|<span data-ttu-id="23521-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23521-174">DateTimeOffset</span></span>|<span data-ttu-id="23521-175">O carimbo de data/hora de quando o script de integridade do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="23521-175">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="23521-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23521-176">This property is read-only.</span></span>|
|<span data-ttu-id="23521-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23521-177">lastModifiedDateTime</span></span>|<span data-ttu-id="23521-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23521-178">DateTimeOffset</span></span>|<span data-ttu-id="23521-179">O carimbo de data/hora de quando o script de integridade do dispositivo foi modificado.</span><span class="sxs-lookup"><span data-stu-id="23521-179">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="23521-180">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23521-180">This property is read-only.</span></span>|
|<span data-ttu-id="23521-181">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="23521-181">runAsAccount</span></span>|[<span data-ttu-id="23521-182">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="23521-182">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="23521-183">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="23521-183">Indicates the type of execution context.</span></span> <span data-ttu-id="23521-184">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="23521-184">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="23521-185">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="23521-185">enforceSignatureCheck</span></span>|<span data-ttu-id="23521-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="23521-186">Boolean</span></span>|<span data-ttu-id="23521-187">Indicar se a assinatura do script precisa ser verificada</span><span class="sxs-lookup"><span data-stu-id="23521-187">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="23521-188">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="23521-188">runAs32Bit</span></span>|<span data-ttu-id="23521-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="23521-189">Boolean</span></span>|<span data-ttu-id="23521-190">Indicar se os scripts do PowerShell devem ser executados como 32 bits</span><span class="sxs-lookup"><span data-stu-id="23521-190">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="23521-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23521-191">roleScopeTagIds</span></span>|<span data-ttu-id="23521-192">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="23521-192">String collection</span></span>|<span data-ttu-id="23521-193">Lista de IDs de marcas de escopo para o script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-193">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="23521-194">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="23521-194">isGlobalScript</span></span>|<span data-ttu-id="23521-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="23521-195">Boolean</span></span>|<span data-ttu-id="23521-196">Determina se este é o script proprietário da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="23521-196">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="23521-197">Scripts proprietários são somente leitura</span><span class="sxs-lookup"><span data-stu-id="23521-197">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="23521-198">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="23521-198">highestAvailableVersion</span></span>|<span data-ttu-id="23521-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23521-199">String</span></span>|<span data-ttu-id="23521-200">Versão mais recente disponível para um script proprietário da Microsoft</span><span class="sxs-lookup"><span data-stu-id="23521-200">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="23521-201">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="23521-201">detectionScriptParameters</span></span>|<span data-ttu-id="23521-202">coleção [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="23521-202">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="23521-203">Lista de objetos complexType DetectionScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="23521-203">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="23521-204">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="23521-204">remediationScriptParameters</span></span>|<span data-ttu-id="23521-205">coleção [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="23521-205">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="23521-206">Lista de objetos complexType RemediationScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="23521-206">List of ComplexType RemediationScriptParameters objects.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23521-207">Relações</span><span class="sxs-lookup"><span data-stu-id="23521-207">Relationships</span></span>
|<span data-ttu-id="23521-208">Relação</span><span class="sxs-lookup"><span data-stu-id="23521-208">Relationship</span></span>|<span data-ttu-id="23521-209">Tipo</span><span class="sxs-lookup"><span data-stu-id="23521-209">Type</span></span>|<span data-ttu-id="23521-210">Descrição</span><span class="sxs-lookup"><span data-stu-id="23521-210">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23521-211">assignments</span><span class="sxs-lookup"><span data-stu-id="23521-211">assignments</span></span>|<span data-ttu-id="23521-212">coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="23521-212">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="23521-213">A lista de atribuições de grupo para o script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23521-213">The list of group assignments for the device health script</span></span>|
|<span data-ttu-id="23521-214">runSummary</span><span class="sxs-lookup"><span data-stu-id="23521-214">runSummary</span></span>|[<span data-ttu-id="23521-215">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="23521-215">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="23521-216">Resumo de execução de alto nível para o script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23521-216">High level run summary for device health script.</span></span>|
|<span data-ttu-id="23521-217">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="23521-217">deviceRunStates</span></span>|<span data-ttu-id="23521-218">coleção [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="23521-218">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="23521-219">Lista de Estados de execução para o script de integridade do dispositivo em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="23521-219">List of run states for the device health script across all devices</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23521-220">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23521-220">JSON Representation</span></span>
<span data-ttu-id="23521-221">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23521-221">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "remediationScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "String",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ]
}
```






