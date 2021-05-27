---
title: Tipo de recurso ticketInfo
description: O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a59b62ddb014dedd802af6fcde001d4791d729c3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682597"
---
# <a name="ticketinfo-resource-type"></a><span data-ttu-id="1c26d-103">Tipo de recurso ticketInfo</span><span class="sxs-lookup"><span data-stu-id="1c26d-103">ticketInfo resource type</span></span>

<span data-ttu-id="1c26d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c26d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c26d-105">O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="1c26d-105">The object that represents ticket information related to role assignment requests</span></span>

## <a name="properties"></a><span data-ttu-id="1c26d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c26d-106">Properties</span></span>
|<span data-ttu-id="1c26d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c26d-107">Property</span></span>|<span data-ttu-id="1c26d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c26d-108">Type</span></span>|<span data-ttu-id="1c26d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c26d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c26d-110">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="1c26d-110">ticketNumber</span></span>|<span data-ttu-id="1c26d-111">String</span><span class="sxs-lookup"><span data-stu-id="1c26d-111">String</span></span>|<span data-ttu-id="1c26d-112">Metadados de número de tíquete</span><span class="sxs-lookup"><span data-stu-id="1c26d-112">Ticket number meta data</span></span>|
|<span data-ttu-id="1c26d-113">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="1c26d-113">ticketSystem</span></span>|<span data-ttu-id="1c26d-114">String</span><span class="sxs-lookup"><span data-stu-id="1c26d-114">String</span></span>|<span data-ttu-id="1c26d-115">Dados de meta do sistema de tíquetes</span><span class="sxs-lookup"><span data-stu-id="1c26d-115">Ticket system meta data</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c26d-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1c26d-116">Relationships</span></span>
<span data-ttu-id="1c26d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c26d-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c26d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c26d-118">JSON representation</span></span>
<span data-ttu-id="1c26d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c26d-119">The following is a JSON representation of the resource.</span></span>
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

