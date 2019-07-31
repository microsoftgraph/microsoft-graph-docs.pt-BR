---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b5ff9da7743a88a1b026826fdd6f2426683bcdc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998342"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="930c2-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="930c2-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="930c2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="930c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="930c2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="930c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="930c2-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="930c2-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="930c2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="930c2-107">Methods</span></span>
|<span data-ttu-id="930c2-108">Método</span><span class="sxs-lookup"><span data-stu-id="930c2-108">Method</span></span>|<span data-ttu-id="930c2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="930c2-109">Return Type</span></span>|<span data-ttu-id="930c2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="930c2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="930c2-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="930c2-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="930c2-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="930c2-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="930c2-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="930c2-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="930c2-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="930c2-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="930c2-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="930c2-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="930c2-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="930c2-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="930c2-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="930c2-117">Properties</span></span>
|<span data-ttu-id="930c2-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="930c2-118">Property</span></span>|<span data-ttu-id="930c2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="930c2-119">Type</span></span>|<span data-ttu-id="930c2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="930c2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="930c2-121">displayName</span><span class="sxs-lookup"><span data-stu-id="930c2-121">displayName</span></span>|<span data-ttu-id="930c2-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="930c2-122">String</span></span>|<span data-ttu-id="930c2-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="930c2-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="930c2-124">id</span><span class="sxs-lookup"><span data-stu-id="930c2-124">id</span></span>|<span data-ttu-id="930c2-125">String</span><span class="sxs-lookup"><span data-stu-id="930c2-125">String</span></span>|<span data-ttu-id="930c2-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="930c2-126">Key of the entity.</span></span>|
|<span data-ttu-id="930c2-127">versão</span><span class="sxs-lookup"><span data-stu-id="930c2-127">version</span></span>|<span data-ttu-id="930c2-128">String</span><span class="sxs-lookup"><span data-stu-id="930c2-128">String</span></span>|<span data-ttu-id="930c2-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="930c2-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="930c2-130">Relações</span><span class="sxs-lookup"><span data-stu-id="930c2-130">Relationships</span></span>
<span data-ttu-id="930c2-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="930c2-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="930c2-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="930c2-132">JSON Representation</span></span>
<span data-ttu-id="930c2-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="930c2-133">Here is a JSON representation of the resource.</span></span>
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





