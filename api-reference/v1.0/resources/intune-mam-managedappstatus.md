---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc6982161e204a4f2e5cac38b62d351ab417482
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258860"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="f4ed0-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f4ed0-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="f4ed0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4ed0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4ed0-105">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="f4ed0-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="f4ed0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4ed0-106">Methods</span></span>
|<span data-ttu-id="f4ed0-107">Método</span><span class="sxs-lookup"><span data-stu-id="f4ed0-107">Method</span></span>|<span data-ttu-id="f4ed0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4ed0-108">Return Type</span></span>|<span data-ttu-id="f4ed0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ed0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4ed0-110">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="f4ed0-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="f4ed0-111">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f4ed0-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="f4ed0-112">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f4ed0-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="f4ed0-113">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f4ed0-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="f4ed0-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f4ed0-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="f4ed0-115">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f4ed0-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4ed0-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4ed0-116">Properties</span></span>
|<span data-ttu-id="f4ed0-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4ed0-117">Property</span></span>|<span data-ttu-id="f4ed0-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ed0-118">Type</span></span>|<span data-ttu-id="f4ed0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ed0-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4ed0-120">displayName</span><span class="sxs-lookup"><span data-stu-id="f4ed0-120">displayName</span></span>|<span data-ttu-id="f4ed0-121">String</span><span class="sxs-lookup"><span data-stu-id="f4ed0-121">String</span></span>|<span data-ttu-id="f4ed0-122">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="f4ed0-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="f4ed0-123">id</span><span class="sxs-lookup"><span data-stu-id="f4ed0-123">id</span></span>|<span data-ttu-id="f4ed0-124">String</span><span class="sxs-lookup"><span data-stu-id="f4ed0-124">String</span></span>|<span data-ttu-id="f4ed0-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4ed0-125">Key of the entity.</span></span>|
|<span data-ttu-id="f4ed0-126">version</span><span class="sxs-lookup"><span data-stu-id="f4ed0-126">version</span></span>|<span data-ttu-id="f4ed0-127">String</span><span class="sxs-lookup"><span data-stu-id="f4ed0-127">String</span></span>|<span data-ttu-id="f4ed0-128">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4ed0-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4ed0-129">Relações</span><span class="sxs-lookup"><span data-stu-id="f4ed0-129">Relationships</span></span>
<span data-ttu-id="f4ed0-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4ed0-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4ed0-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4ed0-131">JSON Representation</span></span>
<span data-ttu-id="f4ed0-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ed0-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



