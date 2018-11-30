---
title: tipo de recurso de synchronizationJobRestartCriteria
description: 'Define o escopo do [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) ação.'
ms.openlocfilehash: edf5cf258750df72dda2c9754d3543e07fc32e39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033547"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="41882-103">tipo de recurso de synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="41882-103">synchronizationJobRestartCriteria resource type</span></span>

> <span data-ttu-id="41882-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="41882-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41882-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41882-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41882-106">Define o escopo do [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) ação.</span><span class="sxs-lookup"><span data-stu-id="41882-106">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="41882-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41882-107">Properties</span></span>
| <span data-ttu-id="41882-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41882-108">Property</span></span>     | <span data-ttu-id="41882-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="41882-109">Type</span></span>   |<span data-ttu-id="41882-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="41882-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41882-111">resetScope</span><span class="sxs-lookup"><span data-stu-id="41882-111">resetScope</span></span>|<span data-ttu-id="41882-112">String</span><span class="sxs-lookup"><span data-stu-id="41882-112">String</span></span>| <span data-ttu-id="41882-113">Combinação de separada por vírgulas dos seguintes valores: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="41882-113">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="41882-114">Uso `Full` se desejar que todas as opções.</span><span class="sxs-lookup"><span data-stu-id="41882-114">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41882-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41882-115">JSON representation</span></span>

<span data-ttu-id="41882-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41882-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->