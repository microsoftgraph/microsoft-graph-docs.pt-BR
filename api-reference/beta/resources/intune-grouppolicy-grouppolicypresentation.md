---
title: tipo de recurso groupPolicyPresentation
description: A entidade base para a apresentação de exibição de qualquer opção adicional em uma definição de política de grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b9ddd53dea0ed2de46f87349f2ea86b3bae086d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259659"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="ae29f-103">tipo de recurso groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="ae29f-103">groupPolicyPresentation resource type</span></span>

<span data-ttu-id="ae29f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae29f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae29f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae29f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae29f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae29f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae29f-107">A entidade base para a apresentação de exibição de qualquer opção adicional em uma definição de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="ae29f-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="ae29f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ae29f-108">Methods</span></span>
|<span data-ttu-id="ae29f-109">Método</span><span class="sxs-lookup"><span data-stu-id="ae29f-109">Method</span></span>|<span data-ttu-id="ae29f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ae29f-110">Return Type</span></span>|<span data-ttu-id="ae29f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae29f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae29f-112">Obter groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="ae29f-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="ae29f-113">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="ae29f-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="ae29f-114">Leia as propriedades e as relações do objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="ae29f-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="ae29f-115">Atualizar groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="ae29f-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="ae29f-116">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="ae29f-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="ae29f-117">Atualiza as propriedades de um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="ae29f-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae29f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae29f-118">Properties</span></span>
|<span data-ttu-id="ae29f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae29f-119">Property</span></span>|<span data-ttu-id="ae29f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae29f-120">Type</span></span>|<span data-ttu-id="ae29f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae29f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae29f-122">rótulo</span><span class="sxs-lookup"><span data-stu-id="ae29f-122">label</span></span>|<span data-ttu-id="ae29f-123">String</span><span class="sxs-lookup"><span data-stu-id="ae29f-123">String</span></span>|<span data-ttu-id="ae29f-124">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="ae29f-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ae29f-125">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ae29f-125">The default value is empty.</span></span>|
|<span data-ttu-id="ae29f-126">id</span><span class="sxs-lookup"><span data-stu-id="ae29f-126">id</span></span>|<span data-ttu-id="ae29f-127">String</span><span class="sxs-lookup"><span data-stu-id="ae29f-127">String</span></span>|<span data-ttu-id="ae29f-128">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ae29f-128">Key of the entity.</span></span>|
|<span data-ttu-id="ae29f-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae29f-129">lastModifiedDateTime</span></span>|<span data-ttu-id="ae29f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae29f-130">DateTimeOffset</span></span>|<span data-ttu-id="ae29f-131">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ae29f-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae29f-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ae29f-132">Relationships</span></span>
|<span data-ttu-id="ae29f-133">Relação</span><span class="sxs-lookup"><span data-stu-id="ae29f-133">Relationship</span></span>|<span data-ttu-id="ae29f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae29f-134">Type</span></span>|<span data-ttu-id="ae29f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae29f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae29f-136">definir</span><span class="sxs-lookup"><span data-stu-id="ae29f-136">definition</span></span>|[<span data-ttu-id="ae29f-137">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="ae29f-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="ae29f-138">A definição de política de grupo associada à apresentação.</span><span class="sxs-lookup"><span data-stu-id="ae29f-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae29f-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae29f-139">JSON Representation</span></span>
<span data-ttu-id="ae29f-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae29f-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




