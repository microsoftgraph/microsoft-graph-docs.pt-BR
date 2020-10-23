---
title: tipo de recurso deviceHealthScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts de integridade do PowerShell (remediation + detecção) nos dispositivos do Windows 10 Azure Active Directory associados registrados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0392140755fb8e57bee27fef113b10bc6ae94b28
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728199"
---
# <a name="devicehealthscript-resource-type"></a><span data-ttu-id="16969-103">tipo de recurso deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-103">deviceHealthScript resource type</span></span>

<span data-ttu-id="16969-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16969-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16969-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16969-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16969-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16969-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16969-107">O Intune fornecerá ao cliente a capacidade de executar os scripts de integridade do PowerShell (remediation + detecção) nos dispositivos do Windows 10 Azure Active Directory associados registrados.</span><span class="sxs-lookup"><span data-stu-id="16969-107">Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.</span></span>

## <a name="methods"></a><span data-ttu-id="16969-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="16969-108">Methods</span></span>
|<span data-ttu-id="16969-109">Método</span><span class="sxs-lookup"><span data-stu-id="16969-109">Method</span></span>|<span data-ttu-id="16969-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16969-110">Return Type</span></span>|<span data-ttu-id="16969-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="16969-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="16969-112">Listar deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="16969-112">List deviceHealthScripts</span></span>](../api/intune-devices-devicehealthscript-list.md)|<span data-ttu-id="16969-113">coleção [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="16969-113">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md) collection</span></span>|<span data-ttu-id="16969-114">Listar Propriedades e relações dos objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="16969-114">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>|
|[<span data-ttu-id="16969-115">Obter deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-115">Get deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-get.md)|[<span data-ttu-id="16969-116">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-116">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="16969-117">Leia as propriedades e as relações do objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="16969-117">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="16969-118">Criar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-118">Create deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-create.md)|[<span data-ttu-id="16969-119">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-119">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="16969-120">Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="16969-120">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="16969-121">Excluir deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-121">Delete deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-delete.md)|<span data-ttu-id="16969-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16969-122">None</span></span>|<span data-ttu-id="16969-123">Exclui [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="16969-123">Deletes a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>|
|[<span data-ttu-id="16969-124">Atualizar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-124">Update deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-update.md)|[<span data-ttu-id="16969-125">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="16969-125">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="16969-126">Atualiza as propriedades de um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="16969-126">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="16969-127">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="16969-127">assign action</span></span>](../api/intune-devices-devicehealthscript-assign.md)|<span data-ttu-id="16969-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="16969-128">None</span></span>|<span data-ttu-id="16969-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="16969-129">Not yet documented</span></span>|
|[<span data-ttu-id="16969-130">ação updateGlobalScript</span><span class="sxs-lookup"><span data-stu-id="16969-130">updateGlobalScript action</span></span>](../api/intune-devices-devicehealthscript-updateglobalscript.md)|<span data-ttu-id="16969-131">String</span><span class="sxs-lookup"><span data-stu-id="16969-131">String</span></span>|<span data-ttu-id="16969-132">Atualizar o script de integridade do dispositivo proprietário</span><span class="sxs-lookup"><span data-stu-id="16969-132">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="16969-133">ação getGlobalScriptHighestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="16969-133">getGlobalScriptHighestAvailableVersion action</span></span>](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|<span data-ttu-id="16969-134">String</span><span class="sxs-lookup"><span data-stu-id="16969-134">String</span></span>|<span data-ttu-id="16969-135">Atualizar o script de integridade do dispositivo proprietário</span><span class="sxs-lookup"><span data-stu-id="16969-135">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="16969-136">ação enableGlobalScripts</span><span class="sxs-lookup"><span data-stu-id="16969-136">enableGlobalScripts action</span></span>](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|<span data-ttu-id="16969-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="16969-137">None</span></span>|<span data-ttu-id="16969-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="16969-138">Not yet documented</span></span>|
|[<span data-ttu-id="16969-139">função areGlobalScriptsAvailable</span><span class="sxs-lookup"><span data-stu-id="16969-139">areGlobalScriptsAvailable function</span></span>](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[<span data-ttu-id="16969-140">globalDeviceHealthScriptState</span><span class="sxs-lookup"><span data-stu-id="16969-140">globalDeviceHealthScriptState</span></span>](../resources/intune-devices-globaldevicehealthscriptstate.md)|<span data-ttu-id="16969-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="16969-141">Not yet documented</span></span>|
|[<span data-ttu-id="16969-142">função getRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="16969-142">getRemediationSummary function</span></span>](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[<span data-ttu-id="16969-143">deviceHealthScriptRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="16969-143">deviceHealthScriptRemediationSummary</span></span>](../resources/intune-devices-devicehealthscriptremediationsummary.md)|<span data-ttu-id="16969-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="16969-144">Not yet documented</span></span>|
|[<span data-ttu-id="16969-145">função getRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="16969-145">getRemediationHistory function</span></span>](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[<span data-ttu-id="16969-146">deviceHealthScriptRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="16969-146">deviceHealthScriptRemediationHistory</span></span>](../resources/intune-devices-devicehealthscriptremediationhistory.md)|<span data-ttu-id="16969-147">Função para obter o número de correções por scripts de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-147">Function to get the number of remediations by a device health scripts</span></span>|

## <a name="properties"></a><span data-ttu-id="16969-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16969-148">Properties</span></span>
|<span data-ttu-id="16969-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16969-149">Property</span></span>|<span data-ttu-id="16969-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="16969-150">Type</span></span>|<span data-ttu-id="16969-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="16969-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16969-152">id</span><span class="sxs-lookup"><span data-stu-id="16969-152">id</span></span>|<span data-ttu-id="16969-153">String</span><span class="sxs-lookup"><span data-stu-id="16969-153">String</span></span>|<span data-ttu-id="16969-154">Identificador exclusivo do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-154">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="16969-155">publicador</span><span class="sxs-lookup"><span data-stu-id="16969-155">publisher</span></span>|<span data-ttu-id="16969-156">String</span><span class="sxs-lookup"><span data-stu-id="16969-156">String</span></span>|<span data-ttu-id="16969-157">Nome do editor de script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-157">Name of the device health script publisher</span></span>|
|<span data-ttu-id="16969-158">versão</span><span class="sxs-lookup"><span data-stu-id="16969-158">version</span></span>|<span data-ttu-id="16969-159">String</span><span class="sxs-lookup"><span data-stu-id="16969-159">String</span></span>|<span data-ttu-id="16969-160">Versão do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-160">Version of the device health script</span></span>|
|<span data-ttu-id="16969-161">displayName</span><span class="sxs-lookup"><span data-stu-id="16969-161">displayName</span></span>|<span data-ttu-id="16969-162">String</span><span class="sxs-lookup"><span data-stu-id="16969-162">String</span></span>|<span data-ttu-id="16969-163">Nome do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-163">Name of the device health script</span></span>|
|<span data-ttu-id="16969-164">description</span><span class="sxs-lookup"><span data-stu-id="16969-164">description</span></span>|<span data-ttu-id="16969-165">String</span><span class="sxs-lookup"><span data-stu-id="16969-165">String</span></span>|<span data-ttu-id="16969-166">Descrição do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-166">Description of the device health script</span></span>|
|<span data-ttu-id="16969-167">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="16969-167">detectionScriptContent</span></span>|<span data-ttu-id="16969-168">Binária</span><span class="sxs-lookup"><span data-stu-id="16969-168">Binary</span></span>|<span data-ttu-id="16969-169">Todo o conteúdo do script do PowerShell de detecção</span><span class="sxs-lookup"><span data-stu-id="16969-169">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="16969-170">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="16969-170">remediationScriptContent</span></span>|<span data-ttu-id="16969-171">Binária</span><span class="sxs-lookup"><span data-stu-id="16969-171">Binary</span></span>|<span data-ttu-id="16969-172">Todo o conteúdo do script do PowerShell de correção</span><span class="sxs-lookup"><span data-stu-id="16969-172">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="16969-173">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16969-173">createdDateTime</span></span>|<span data-ttu-id="16969-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16969-174">DateTimeOffset</span></span>|<span data-ttu-id="16969-175">O carimbo de data/hora de quando o script de integridade do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="16969-175">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="16969-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16969-176">This property is read-only.</span></span>|
|<span data-ttu-id="16969-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16969-177">lastModifiedDateTime</span></span>|<span data-ttu-id="16969-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16969-178">DateTimeOffset</span></span>|<span data-ttu-id="16969-179">O carimbo de data/hora de quando o script de integridade do dispositivo foi modificado.</span><span class="sxs-lookup"><span data-stu-id="16969-179">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="16969-180">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16969-180">This property is read-only.</span></span>|
|<span data-ttu-id="16969-181">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="16969-181">runAsAccount</span></span>|[<span data-ttu-id="16969-182">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="16969-182">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="16969-183">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="16969-183">Indicates the type of execution context.</span></span> <span data-ttu-id="16969-184">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="16969-184">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="16969-185">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="16969-185">enforceSignatureCheck</span></span>|<span data-ttu-id="16969-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="16969-186">Boolean</span></span>|<span data-ttu-id="16969-187">Indicar se a assinatura do script precisa ser verificada</span><span class="sxs-lookup"><span data-stu-id="16969-187">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="16969-188">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="16969-188">runAs32Bit</span></span>|<span data-ttu-id="16969-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="16969-189">Boolean</span></span>|<span data-ttu-id="16969-190">Indicar se os scripts do PowerShell devem ser executados como 32 bits</span><span class="sxs-lookup"><span data-stu-id="16969-190">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="16969-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16969-191">roleScopeTagIds</span></span>|<span data-ttu-id="16969-192">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="16969-192">String collection</span></span>|<span data-ttu-id="16969-193">Lista de IDs de marcas de escopo para o script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-193">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="16969-194">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="16969-194">isGlobalScript</span></span>|<span data-ttu-id="16969-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="16969-195">Boolean</span></span>|<span data-ttu-id="16969-196">Determina se este é o script proprietário da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="16969-196">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="16969-197">Scripts proprietários são somente leitura</span><span class="sxs-lookup"><span data-stu-id="16969-197">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="16969-198">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="16969-198">highestAvailableVersion</span></span>|<span data-ttu-id="16969-199">String</span><span class="sxs-lookup"><span data-stu-id="16969-199">String</span></span>|<span data-ttu-id="16969-200">Versão mais recente disponível para um script proprietário da Microsoft</span><span class="sxs-lookup"><span data-stu-id="16969-200">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="16969-201">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="16969-201">detectionScriptParameters</span></span>|<span data-ttu-id="16969-202">coleção [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="16969-202">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="16969-203">Lista de objetos complexType DetectionScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="16969-203">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="16969-204">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="16969-204">remediationScriptParameters</span></span>|<span data-ttu-id="16969-205">coleção [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="16969-205">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="16969-206">Lista de objetos complexType RemediationScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="16969-206">List of ComplexType RemediationScriptParameters objects.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16969-207">Relações</span><span class="sxs-lookup"><span data-stu-id="16969-207">Relationships</span></span>
|<span data-ttu-id="16969-208">Relação</span><span class="sxs-lookup"><span data-stu-id="16969-208">Relationship</span></span>|<span data-ttu-id="16969-209">Tipo</span><span class="sxs-lookup"><span data-stu-id="16969-209">Type</span></span>|<span data-ttu-id="16969-210">Descrição</span><span class="sxs-lookup"><span data-stu-id="16969-210">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16969-211">assignments</span><span class="sxs-lookup"><span data-stu-id="16969-211">assignments</span></span>|<span data-ttu-id="16969-212">coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="16969-212">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="16969-213">A lista de atribuições de grupo para o script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16969-213">The list of group assignments for the device health script</span></span>|
|<span data-ttu-id="16969-214">runSummary</span><span class="sxs-lookup"><span data-stu-id="16969-214">runSummary</span></span>|[<span data-ttu-id="16969-215">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="16969-215">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="16969-216">Resumo de execução de alto nível para o script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16969-216">High level run summary for device health script.</span></span>|
|<span data-ttu-id="16969-217">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="16969-217">deviceRunStates</span></span>|<span data-ttu-id="16969-218">coleção [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="16969-218">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="16969-219">Lista de Estados de execução para o script de integridade do dispositivo em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="16969-219">List of run states for the device health script across all devices</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16969-220">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16969-220">JSON Representation</span></span>
<span data-ttu-id="16969-221">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16969-221">Here is a JSON representation of the resource.</span></span>
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





