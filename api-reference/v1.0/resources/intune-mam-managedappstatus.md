---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: deaca18dd8a11c930bdd052a6e3c1f94f0de1a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448323"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="43700-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="43700-103">managedAppStatus resource type</span></span>

<span data-ttu-id="43700-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="43700-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43700-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43700-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43700-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="43700-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="43700-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="43700-107">Methods</span></span>
|<span data-ttu-id="43700-108">Método</span><span class="sxs-lookup"><span data-stu-id="43700-108">Method</span></span>|<span data-ttu-id="43700-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43700-109">Return Type</span></span>|<span data-ttu-id="43700-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43700-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43700-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="43700-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="43700-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="43700-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="43700-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="43700-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="43700-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="43700-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="43700-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="43700-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="43700-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="43700-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43700-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43700-117">Properties</span></span>
|<span data-ttu-id="43700-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43700-118">Property</span></span>|<span data-ttu-id="43700-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="43700-119">Type</span></span>|<span data-ttu-id="43700-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="43700-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43700-121">displayName</span><span class="sxs-lookup"><span data-stu-id="43700-121">displayName</span></span>|<span data-ttu-id="43700-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43700-122">String</span></span>|<span data-ttu-id="43700-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="43700-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="43700-124">id</span><span class="sxs-lookup"><span data-stu-id="43700-124">id</span></span>|<span data-ttu-id="43700-125">String</span><span class="sxs-lookup"><span data-stu-id="43700-125">String</span></span>|<span data-ttu-id="43700-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="43700-126">Key of the entity.</span></span>|
|<span data-ttu-id="43700-127">versão</span><span class="sxs-lookup"><span data-stu-id="43700-127">version</span></span>|<span data-ttu-id="43700-128">String</span><span class="sxs-lookup"><span data-stu-id="43700-128">String</span></span>|<span data-ttu-id="43700-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="43700-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43700-130">Relações</span><span class="sxs-lookup"><span data-stu-id="43700-130">Relationships</span></span>
<span data-ttu-id="43700-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43700-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43700-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43700-132">JSON Representation</span></span>
<span data-ttu-id="43700-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43700-133">Here is a JSON representation of the resource.</span></span>
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




