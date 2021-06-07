---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 034a7961cedb5fe6e73ce4ac04774e6c64596428
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751654"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="f3b16-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f3b16-103">managedAppStatus resource type</span></span>

<span data-ttu-id="f3b16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3b16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3b16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3b16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3b16-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="f3b16-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="f3b16-107">Methods</span><span class="sxs-lookup"><span data-stu-id="f3b16-107">Methods</span></span>
|<span data-ttu-id="f3b16-108">Método</span><span class="sxs-lookup"><span data-stu-id="f3b16-108">Method</span></span>|<span data-ttu-id="f3b16-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3b16-109">Return Type</span></span>|<span data-ttu-id="f3b16-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3b16-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3b16-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="f3b16-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="f3b16-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f3b16-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="f3b16-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f3b16-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="f3b16-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f3b16-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="f3b16-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f3b16-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="f3b16-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f3b16-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3b16-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3b16-117">Properties</span></span>
|<span data-ttu-id="f3b16-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3b16-118">Property</span></span>|<span data-ttu-id="f3b16-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3b16-119">Type</span></span>|<span data-ttu-id="f3b16-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3b16-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b16-121">displayName</span><span class="sxs-lookup"><span data-stu-id="f3b16-121">displayName</span></span>|<span data-ttu-id="f3b16-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3b16-122">String</span></span>|<span data-ttu-id="f3b16-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="f3b16-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="f3b16-124">id</span><span class="sxs-lookup"><span data-stu-id="f3b16-124">id</span></span>|<span data-ttu-id="f3b16-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3b16-125">String</span></span>|<span data-ttu-id="f3b16-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3b16-126">Key of the entity.</span></span>|
|<span data-ttu-id="f3b16-127">versão</span><span class="sxs-lookup"><span data-stu-id="f3b16-127">version</span></span>|<span data-ttu-id="f3b16-128">String</span><span class="sxs-lookup"><span data-stu-id="f3b16-128">String</span></span>|<span data-ttu-id="f3b16-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3b16-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3b16-130">Relações</span><span class="sxs-lookup"><span data-stu-id="f3b16-130">Relationships</span></span>
<span data-ttu-id="f3b16-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f3b16-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3b16-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3b16-132">JSON Representation</span></span>
<span data-ttu-id="f3b16-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3b16-133">Here is a JSON representation of the resource.</span></span>
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




