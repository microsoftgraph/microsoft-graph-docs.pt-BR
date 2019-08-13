---
title: tipo de recurso groupPolicyPresentation
description: A entidade base para a apresentação de exibição de qualquer opção adicional em uma definição de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ee950b7e4e292b9fb177778ff4df2dcb51641e54
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331431"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="a925b-103">tipo de recurso groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="a925b-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="a925b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a925b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a925b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a925b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a925b-106">A entidade base para a apresentação de exibição de qualquer opção adicional em uma definição de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a925b-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="a925b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a925b-107">Methods</span></span>
|<span data-ttu-id="a925b-108">Método</span><span class="sxs-lookup"><span data-stu-id="a925b-108">Method</span></span>|<span data-ttu-id="a925b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a925b-109">Return Type</span></span>|<span data-ttu-id="a925b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a925b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a925b-111">Obter groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="a925b-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="a925b-112">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="a925b-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="a925b-113">Leia as propriedades e as relações do objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="a925b-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="a925b-114">Atualizar groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="a925b-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="a925b-115">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="a925b-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="a925b-116">Atualiza as propriedades de um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="a925b-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a925b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a925b-117">Properties</span></span>
|<span data-ttu-id="a925b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a925b-118">Property</span></span>|<span data-ttu-id="a925b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a925b-119">Type</span></span>|<span data-ttu-id="a925b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a925b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a925b-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="a925b-121">label</span></span>|<span data-ttu-id="a925b-122">String</span><span class="sxs-lookup"><span data-stu-id="a925b-122">String</span></span>|<span data-ttu-id="a925b-123">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="a925b-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a925b-124">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="a925b-124">The default value is empty.</span></span>|
|<span data-ttu-id="a925b-125">id</span><span class="sxs-lookup"><span data-stu-id="a925b-125">id</span></span>|<span data-ttu-id="a925b-126">String</span><span class="sxs-lookup"><span data-stu-id="a925b-126">String</span></span>|<span data-ttu-id="a925b-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a925b-127">Key of the entity.</span></span>|
|<span data-ttu-id="a925b-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a925b-128">lastModifiedDateTime</span></span>|<span data-ttu-id="a925b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a925b-129">DateTimeOffset</span></span>|<span data-ttu-id="a925b-130">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a925b-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a925b-131">Relações</span><span class="sxs-lookup"><span data-stu-id="a925b-131">Relationships</span></span>
|<span data-ttu-id="a925b-132">Relação</span><span class="sxs-lookup"><span data-stu-id="a925b-132">Relationship</span></span>|<span data-ttu-id="a925b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a925b-133">Type</span></span>|<span data-ttu-id="a925b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a925b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a925b-135">definir</span><span class="sxs-lookup"><span data-stu-id="a925b-135">definition</span></span>|[<span data-ttu-id="a925b-136">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a925b-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="a925b-137">A definição de política de grupo associada à apresentação.</span><span class="sxs-lookup"><span data-stu-id="a925b-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a925b-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a925b-138">JSON Representation</span></span>
<span data-ttu-id="a925b-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a925b-139">Here is a JSON representation of the resource.</span></span>
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



