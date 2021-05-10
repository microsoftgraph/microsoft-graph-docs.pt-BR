---
title: Tipo de recurso ticketInfo
description: O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 584600bf017a75efb141539b6f1397920717fb76
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299081"
---
# <a name="ticketinfo-resource-type"></a><span data-ttu-id="69453-103">Tipo de recurso ticketInfo</span><span class="sxs-lookup"><span data-stu-id="69453-103">ticketInfo resource type</span></span>

<span data-ttu-id="69453-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69453-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69453-105">O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="69453-105">The object that represents ticket information related to role assignment requests</span></span>

## <a name="properties"></a><span data-ttu-id="69453-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69453-106">Properties</span></span>
|<span data-ttu-id="69453-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69453-107">Property</span></span>|<span data-ttu-id="69453-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="69453-108">Type</span></span>|<span data-ttu-id="69453-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="69453-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69453-110">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="69453-110">ticketNumber</span></span>|<span data-ttu-id="69453-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69453-111">String</span></span>|<span data-ttu-id="69453-112">Metadados de número de tíquete</span><span class="sxs-lookup"><span data-stu-id="69453-112">Ticket number meta data</span></span>|
|<span data-ttu-id="69453-113">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="69453-113">ticketSystem</span></span>|<span data-ttu-id="69453-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69453-114">String</span></span>|<span data-ttu-id="69453-115">Dados de meta do sistema de tíquetes</span><span class="sxs-lookup"><span data-stu-id="69453-115">Ticket system meta data</span></span>|

## <a name="relationships"></a><span data-ttu-id="69453-116">Relações</span><span class="sxs-lookup"><span data-stu-id="69453-116">Relationships</span></span>
<span data-ttu-id="69453-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69453-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69453-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69453-118">JSON representation</span></span>
<span data-ttu-id="69453-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69453-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ticketInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ticketInfo",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

