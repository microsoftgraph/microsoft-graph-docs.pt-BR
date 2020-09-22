---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f8d41d1768f843ea5d2c6e4c61256cdfbc1d629
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988230"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="e605c-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="e605c-103">managedAppStatus resource type</span></span>

<span data-ttu-id="e605c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e605c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e605c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e605c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e605c-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="e605c-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="e605c-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e605c-107">Methods</span></span>
|<span data-ttu-id="e605c-108">Método</span><span class="sxs-lookup"><span data-stu-id="e605c-108">Method</span></span>|<span data-ttu-id="e605c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e605c-109">Return Type</span></span>|<span data-ttu-id="e605c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e605c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e605c-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="e605c-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="e605c-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="e605c-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="e605c-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e605c-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="e605c-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="e605c-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="e605c-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="e605c-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="e605c-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e605c-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e605c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e605c-117">Properties</span></span>
|<span data-ttu-id="e605c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e605c-118">Property</span></span>|<span data-ttu-id="e605c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e605c-119">Type</span></span>|<span data-ttu-id="e605c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e605c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e605c-121">displayName</span><span class="sxs-lookup"><span data-stu-id="e605c-121">displayName</span></span>|<span data-ttu-id="e605c-122">String</span><span class="sxs-lookup"><span data-stu-id="e605c-122">String</span></span>|<span data-ttu-id="e605c-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="e605c-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="e605c-124">id</span><span class="sxs-lookup"><span data-stu-id="e605c-124">id</span></span>|<span data-ttu-id="e605c-125">String</span><span class="sxs-lookup"><span data-stu-id="e605c-125">String</span></span>|<span data-ttu-id="e605c-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e605c-126">Key of the entity.</span></span>|
|<span data-ttu-id="e605c-127">versão</span><span class="sxs-lookup"><span data-stu-id="e605c-127">version</span></span>|<span data-ttu-id="e605c-128">String</span><span class="sxs-lookup"><span data-stu-id="e605c-128">String</span></span>|<span data-ttu-id="e605c-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="e605c-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e605c-130">Relações</span><span class="sxs-lookup"><span data-stu-id="e605c-130">Relationships</span></span>
<span data-ttu-id="e605c-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e605c-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e605c-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e605c-132">JSON Representation</span></span>
<span data-ttu-id="e605c-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e605c-133">Here is a JSON representation of the resource.</span></span>
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









