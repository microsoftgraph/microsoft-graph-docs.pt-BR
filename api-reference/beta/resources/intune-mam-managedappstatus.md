---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 523d564f00189952ac3046c5f02bf782bc0f8e2f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371787"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="7f2f7-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7f2f7-103">managedAppStatus resource type</span></span>

<span data-ttu-id="7f2f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f2f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f2f7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f2f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f2f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f2f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f2f7-107">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="7f2f7-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="7f2f7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f2f7-108">Methods</span></span>
|<span data-ttu-id="7f2f7-109">Método</span><span class="sxs-lookup"><span data-stu-id="7f2f7-109">Method</span></span>|<span data-ttu-id="7f2f7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f2f7-110">Return Type</span></span>|<span data-ttu-id="7f2f7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f2f7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f2f7-112">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="7f2f7-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="7f2f7-113">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7f2f7-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="7f2f7-114">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7f2f7-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="7f2f7-115">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7f2f7-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="7f2f7-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7f2f7-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="7f2f7-117">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7f2f7-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f2f7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f2f7-118">Properties</span></span>
|<span data-ttu-id="7f2f7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f2f7-119">Property</span></span>|<span data-ttu-id="7f2f7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f2f7-120">Type</span></span>|<span data-ttu-id="7f2f7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f2f7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f2f7-122">displayName</span><span class="sxs-lookup"><span data-stu-id="7f2f7-122">displayName</span></span>|<span data-ttu-id="7f2f7-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f2f7-123">String</span></span>|<span data-ttu-id="7f2f7-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="7f2f7-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="7f2f7-125">id</span><span class="sxs-lookup"><span data-stu-id="7f2f7-125">id</span></span>|<span data-ttu-id="7f2f7-126">String</span><span class="sxs-lookup"><span data-stu-id="7f2f7-126">String</span></span>|<span data-ttu-id="7f2f7-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7f2f7-127">Key of the entity.</span></span>|
|<span data-ttu-id="7f2f7-128">versão</span><span class="sxs-lookup"><span data-stu-id="7f2f7-128">version</span></span>|<span data-ttu-id="7f2f7-129">String</span><span class="sxs-lookup"><span data-stu-id="7f2f7-129">String</span></span>|<span data-ttu-id="7f2f7-130">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="7f2f7-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f2f7-131">Relações</span><span class="sxs-lookup"><span data-stu-id="7f2f7-131">Relationships</span></span>
<span data-ttu-id="7f2f7-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f2f7-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f2f7-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f2f7-133">JSON Representation</span></span>
<span data-ttu-id="7f2f7-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f2f7-134">Here is a JSON representation of the resource.</span></span>
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



