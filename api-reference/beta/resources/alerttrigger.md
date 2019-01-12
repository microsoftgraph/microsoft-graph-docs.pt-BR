---
title: tipo de recurso de alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 56034fb566f960ec858b86cdb4bcac86e5b9b47a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946424"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="7a82c-104">tipo de recurso de alertTrigger</span><span class="sxs-lookup"><span data-stu-id="7a82c-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="7a82c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7a82c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a82c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7a82c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a82c-107">Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).</span><span class="sxs-lookup"><span data-stu-id="7a82c-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="7a82c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a82c-108">Properties</span></span>

| <span data-ttu-id="7a82c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a82c-109">Property</span></span>   | <span data-ttu-id="7a82c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a82c-110">Type</span></span>|<span data-ttu-id="7a82c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a82c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a82c-112">name</span><span class="sxs-lookup"><span data-stu-id="7a82c-112">name</span></span>|<span data-ttu-id="7a82c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a82c-113">String</span></span>|<span data-ttu-id="7a82c-114">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="7a82c-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="7a82c-115">type</span><span class="sxs-lookup"><span data-stu-id="7a82c-115">type</span></span>|<span data-ttu-id="7a82c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a82c-116">String</span></span>|<span data-ttu-id="7a82c-117">Tipo da propriedade no par de chave: valor de interpretação.</span><span class="sxs-lookup"><span data-stu-id="7a82c-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="7a82c-118">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="7a82c-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="7a82c-119">valor</span><span class="sxs-lookup"><span data-stu-id="7a82c-119">value</span></span>|<span data-ttu-id="7a82c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a82c-120">String</span></span>|<span data-ttu-id="7a82c-121">Valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="7a82c-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a82c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a82c-122">JSON representation</span></span>

<span data-ttu-id="7a82c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a82c-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="7a82c-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a82c-124">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
