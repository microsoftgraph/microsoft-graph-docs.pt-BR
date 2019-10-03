---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 178bc51d6293947f425dd3580a0bc9f9af208f7c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367025"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="89a22-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="89a22-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="89a22-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89a22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89a22-105">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="89a22-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="89a22-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="89a22-106">Methods</span></span>
|<span data-ttu-id="89a22-107">Método</span><span class="sxs-lookup"><span data-stu-id="89a22-107">Method</span></span>|<span data-ttu-id="89a22-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="89a22-108">Return Type</span></span>|<span data-ttu-id="89a22-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89a22-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89a22-110">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="89a22-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="89a22-111">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="89a22-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="89a22-112">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="89a22-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="89a22-113">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="89a22-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="89a22-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="89a22-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="89a22-115">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="89a22-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89a22-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89a22-116">Properties</span></span>
|<span data-ttu-id="89a22-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89a22-117">Property</span></span>|<span data-ttu-id="89a22-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="89a22-118">Type</span></span>|<span data-ttu-id="89a22-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="89a22-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a22-120">displayName</span><span class="sxs-lookup"><span data-stu-id="89a22-120">displayName</span></span>|<span data-ttu-id="89a22-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89a22-121">String</span></span>|<span data-ttu-id="89a22-122">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="89a22-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="89a22-123">id</span><span class="sxs-lookup"><span data-stu-id="89a22-123">id</span></span>|<span data-ttu-id="89a22-124">String</span><span class="sxs-lookup"><span data-stu-id="89a22-124">String</span></span>|<span data-ttu-id="89a22-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="89a22-125">Key of the entity.</span></span>|
|<span data-ttu-id="89a22-126">versão</span><span class="sxs-lookup"><span data-stu-id="89a22-126">version</span></span>|<span data-ttu-id="89a22-127">String</span><span class="sxs-lookup"><span data-stu-id="89a22-127">String</span></span>|<span data-ttu-id="89a22-128">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="89a22-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89a22-129">Relações</span><span class="sxs-lookup"><span data-stu-id="89a22-129">Relationships</span></span>
<span data-ttu-id="89a22-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89a22-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89a22-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89a22-131">JSON Representation</span></span>
<span data-ttu-id="89a22-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89a22-132">Here is a JSON representation of the resource.</span></span>
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




