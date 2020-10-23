---
title: tipo de recurso managementConditionStatement
description: Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que Habilita/desabilita as configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidas são atendidas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5bebd514c4a24bd9a19b1a23c5b354c330d2bdf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722841"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="ca7d5-103">tipo de recurso managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-103">managementConditionStatement resource type</span></span>

<span data-ttu-id="ca7d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca7d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca7d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca7d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca7d5-107">Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que Habilita/desabilita as configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidas são atendidas.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-107">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>

## <a name="methods"></a><span data-ttu-id="ca7d5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ca7d5-108">Methods</span></span>
|<span data-ttu-id="ca7d5-109">Método</span><span class="sxs-lookup"><span data-stu-id="ca7d5-109">Method</span></span>|<span data-ttu-id="ca7d5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ca7d5-110">Return Type</span></span>|<span data-ttu-id="ca7d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca7d5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca7d5-112">Listar managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="ca7d5-112">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="ca7d5-113">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="ca7d5-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="ca7d5-114">Listar Propriedades e relações dos objetos [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="ca7d5-114">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="ca7d5-115">Obter managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-115">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="ca7d5-116">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-116">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="ca7d5-117">Leia as propriedades e as relações do objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="ca7d5-117">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="ca7d5-118">Criar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-118">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="ca7d5-119">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-119">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="ca7d5-120">Criar um novo objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="ca7d5-120">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="ca7d5-121">Excluir managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-121">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="ca7d5-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca7d5-122">None</span></span>|<span data-ttu-id="ca7d5-123">Exclui [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="ca7d5-123">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="ca7d5-124">Atualizar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-124">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="ca7d5-125">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="ca7d5-125">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="ca7d5-126">Atualiza as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="ca7d5-126">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="ca7d5-127">função getManagementConditionStatementExpressionString</span><span class="sxs-lookup"><span data-stu-id="ca7d5-127">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="ca7d5-128">managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="ca7d5-128">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="ca7d5-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ca7d5-129">Not yet documented</span></span>|
|[<span data-ttu-id="ca7d5-130">função getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="ca7d5-130">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="ca7d5-131">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="ca7d5-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="ca7d5-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ca7d5-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ca7d5-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca7d5-133">Properties</span></span>
|<span data-ttu-id="ca7d5-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca7d5-134">Property</span></span>|<span data-ttu-id="ca7d5-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca7d5-135">Type</span></span>|<span data-ttu-id="ca7d5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca7d5-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca7d5-137">id</span><span class="sxs-lookup"><span data-stu-id="ca7d5-137">id</span></span>|<span data-ttu-id="ca7d5-138">String</span><span class="sxs-lookup"><span data-stu-id="ca7d5-138">String</span></span>|<span data-ttu-id="ca7d5-139">Identificador exclusivo da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-139">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="ca7d5-140">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-140">System generated value assigned when created.</span></span>|
|<span data-ttu-id="ca7d5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ca7d5-141">displayName</span></span>|<span data-ttu-id="ca7d5-142">String</span><span class="sxs-lookup"><span data-stu-id="ca7d5-142">String</span></span>|<span data-ttu-id="ca7d5-143">O nome do administrador definido da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-143">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="ca7d5-144">description</span><span class="sxs-lookup"><span data-stu-id="ca7d5-144">description</span></span>|<span data-ttu-id="ca7d5-145">String</span><span class="sxs-lookup"><span data-stu-id="ca7d5-145">String</span></span>|<span data-ttu-id="ca7d5-146">A descrição definida pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-146">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="ca7d5-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca7d5-147">createdDateTime</span></span>|<span data-ttu-id="ca7d5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca7d5-148">DateTimeOffset</span></span>|<span data-ttu-id="ca7d5-149">A hora em que a instrução de gerenciamento da condição foi criada.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-149">The time the management condition statement was created.</span></span> <span data-ttu-id="ca7d5-150">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-150">Generated service side.</span></span>|
|<span data-ttu-id="ca7d5-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca7d5-151">modifiedDateTime</span></span>|<span data-ttu-id="ca7d5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca7d5-152">DateTimeOffset</span></span>|<span data-ttu-id="ca7d5-153">A hora em que a declaração de condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-153">The time the management condition statement was last modified.</span></span> <span data-ttu-id="ca7d5-154">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-154">Updated service side.</span></span>|
|<span data-ttu-id="ca7d5-155">expressão</span><span class="sxs-lookup"><span data-stu-id="ca7d5-155">expression</span></span>|[<span data-ttu-id="ca7d5-156">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="ca7d5-156">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="ca7d5-157">A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-157">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="ca7d5-158">eTag</span><span class="sxs-lookup"><span data-stu-id="ca7d5-158">eTag</span></span>|<span data-ttu-id="ca7d5-159">String</span><span class="sxs-lookup"><span data-stu-id="ca7d5-159">String</span></span>|<span data-ttu-id="ca7d5-160">ETag da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-160">ETag of the management condition statement.</span></span> <span data-ttu-id="ca7d5-161">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-161">Updated service side.</span></span>|
|<span data-ttu-id="ca7d5-162">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="ca7d5-162">applicablePlatforms</span></span>|<span data-ttu-id="ca7d5-163">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="ca7d5-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="ca7d5-164">As plataformas aplicáveis para essa instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-164">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="ca7d5-165">Isso é calculado a partir da aparência das condições de gerenciamento associadas à instrução de condição de gerenciamento e à localização da interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-165">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca7d5-166">Relações</span><span class="sxs-lookup"><span data-stu-id="ca7d5-166">Relationships</span></span>
|<span data-ttu-id="ca7d5-167">Relação</span><span class="sxs-lookup"><span data-stu-id="ca7d5-167">Relationship</span></span>|<span data-ttu-id="ca7d5-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca7d5-168">Type</span></span>|<span data-ttu-id="ca7d5-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca7d5-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca7d5-170">managementConditions</span><span class="sxs-lookup"><span data-stu-id="ca7d5-170">managementConditions</span></span>|<span data-ttu-id="ca7d5-171">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7d5-171">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="ca7d5-172">As condições de gerenciamento associadas à instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-172">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca7d5-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca7d5-173">JSON Representation</span></span>
<span data-ttu-id="ca7d5-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca7d5-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "String"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





