---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc9f6596e9d9361a8c211809bf0f621fe36bcd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153155"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="8d4dd-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8d4dd-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="8d4dd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d4dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d4dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d4dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d4dd-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="8d4dd-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="8d4dd-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d4dd-107">Methods</span></span>
|<span data-ttu-id="8d4dd-108">Método</span><span class="sxs-lookup"><span data-stu-id="8d4dd-108">Method</span></span>|<span data-ttu-id="8d4dd-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d4dd-109">Return Type</span></span>|<span data-ttu-id="8d4dd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d4dd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8d4dd-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="8d4dd-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="8d4dd-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8d4dd-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="8d4dd-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8d4dd-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="8d4dd-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8d4dd-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="8d4dd-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8d4dd-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="8d4dd-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8d4dd-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d4dd-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d4dd-117">Properties</span></span>
|<span data-ttu-id="8d4dd-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d4dd-118">Property</span></span>|<span data-ttu-id="8d4dd-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d4dd-119">Type</span></span>|<span data-ttu-id="8d4dd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d4dd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d4dd-121">displayName</span><span class="sxs-lookup"><span data-stu-id="8d4dd-121">displayName</span></span>|<span data-ttu-id="8d4dd-122">String</span><span class="sxs-lookup"><span data-stu-id="8d4dd-122">String</span></span>|<span data-ttu-id="8d4dd-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="8d4dd-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="8d4dd-124">id</span><span class="sxs-lookup"><span data-stu-id="8d4dd-124">id</span></span>|<span data-ttu-id="8d4dd-125">String</span><span class="sxs-lookup"><span data-stu-id="8d4dd-125">String</span></span>|<span data-ttu-id="8d4dd-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d4dd-126">Key of the entity.</span></span>|
|<span data-ttu-id="8d4dd-127">version</span><span class="sxs-lookup"><span data-stu-id="8d4dd-127">version</span></span>|<span data-ttu-id="8d4dd-128">String</span><span class="sxs-lookup"><span data-stu-id="8d4dd-128">String</span></span>|<span data-ttu-id="8d4dd-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d4dd-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d4dd-130">Relações</span><span class="sxs-lookup"><span data-stu-id="8d4dd-130">Relationships</span></span>
<span data-ttu-id="8d4dd-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d4dd-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d4dd-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d4dd-132">JSON Representation</span></span>
<span data-ttu-id="8d4dd-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d4dd-133">Here is a JSON representation of the resource.</span></span>
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




