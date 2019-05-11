---
title: tipo de recurso groupPolicyPresentation
description: A entidade base para a apresentação de exibição de qualquer opção adicional em uma definição de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8a1e4a615999a899712ad82d2177fbb862328c2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941125"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="d51d0-103">tipo de recurso groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="d51d0-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="d51d0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d51d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d51d0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d51d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d51d0-106">A entidade base para a apresentação de exibição de qualquer opção adicional em uma definição de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="d51d0-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="d51d0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d51d0-107">Methods</span></span>
|<span data-ttu-id="d51d0-108">Método</span><span class="sxs-lookup"><span data-stu-id="d51d0-108">Method</span></span>|<span data-ttu-id="d51d0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d51d0-109">Return Type</span></span>|<span data-ttu-id="d51d0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d51d0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d51d0-111">Obter groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="d51d0-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="d51d0-112">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="d51d0-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="d51d0-113">Leia as propriedades e as relações do objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="d51d0-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="d51d0-114">Atualizar groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="d51d0-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="d51d0-115">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="d51d0-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="d51d0-116">Atualiza as propriedades de um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="d51d0-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d51d0-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d51d0-117">Properties</span></span>
|<span data-ttu-id="d51d0-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d51d0-118">Property</span></span>|<span data-ttu-id="d51d0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d51d0-119">Type</span></span>|<span data-ttu-id="d51d0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d51d0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d51d0-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="d51d0-121">label</span></span>|<span data-ttu-id="d51d0-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d51d0-122">String</span></span>|<span data-ttu-id="d51d0-123">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="d51d0-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d51d0-124">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="d51d0-124">The default value is empty.</span></span>|
|<span data-ttu-id="d51d0-125">id</span><span class="sxs-lookup"><span data-stu-id="d51d0-125">id</span></span>|<span data-ttu-id="d51d0-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d51d0-126">String</span></span>|<span data-ttu-id="d51d0-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d51d0-127">Key of the entity.</span></span>|
|<span data-ttu-id="d51d0-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d51d0-128">lastModifiedDateTime</span></span>|<span data-ttu-id="d51d0-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d51d0-129">DateTimeOffset</span></span>|<span data-ttu-id="d51d0-130">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d51d0-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d51d0-131">Relações</span><span class="sxs-lookup"><span data-stu-id="d51d0-131">Relationships</span></span>
|<span data-ttu-id="d51d0-132">Relação</span><span class="sxs-lookup"><span data-stu-id="d51d0-132">Relationship</span></span>|<span data-ttu-id="d51d0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d51d0-133">Type</span></span>|<span data-ttu-id="d51d0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d51d0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d51d0-135">definir</span><span class="sxs-lookup"><span data-stu-id="d51d0-135">definition</span></span>|[<span data-ttu-id="d51d0-136">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="d51d0-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="d51d0-137">A definição de política de grupo associada à apresentação.</span><span class="sxs-lookup"><span data-stu-id="d51d0-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d51d0-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d51d0-138">JSON Representation</span></span>
<span data-ttu-id="d51d0-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d51d0-139">Here is a JSON representation of the resource.</span></span>
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




