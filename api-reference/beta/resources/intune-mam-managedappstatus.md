---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b2503ea58e57a0a91af6e2d0e07ac394c04957b1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373081"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="24779-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="24779-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="24779-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24779-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24779-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24779-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24779-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="24779-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="24779-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="24779-107">Methods</span></span>
|<span data-ttu-id="24779-108">Método</span><span class="sxs-lookup"><span data-stu-id="24779-108">Method</span></span>|<span data-ttu-id="24779-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="24779-109">Return Type</span></span>|<span data-ttu-id="24779-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="24779-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24779-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="24779-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="24779-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="24779-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="24779-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="24779-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="24779-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="24779-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="24779-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="24779-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="24779-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="24779-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="24779-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24779-117">Properties</span></span>
|<span data-ttu-id="24779-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24779-118">Property</span></span>|<span data-ttu-id="24779-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="24779-119">Type</span></span>|<span data-ttu-id="24779-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="24779-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24779-121">displayName</span><span class="sxs-lookup"><span data-stu-id="24779-121">displayName</span></span>|<span data-ttu-id="24779-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24779-122">String</span></span>|<span data-ttu-id="24779-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="24779-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="24779-124">id</span><span class="sxs-lookup"><span data-stu-id="24779-124">id</span></span>|<span data-ttu-id="24779-125">String</span><span class="sxs-lookup"><span data-stu-id="24779-125">String</span></span>|<span data-ttu-id="24779-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="24779-126">Key of the entity.</span></span>|
|<span data-ttu-id="24779-127">versão</span><span class="sxs-lookup"><span data-stu-id="24779-127">version</span></span>|<span data-ttu-id="24779-128">String</span><span class="sxs-lookup"><span data-stu-id="24779-128">String</span></span>|<span data-ttu-id="24779-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="24779-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24779-130">Relações</span><span class="sxs-lookup"><span data-stu-id="24779-130">Relationships</span></span>
<span data-ttu-id="24779-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24779-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24779-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24779-132">JSON Representation</span></span>
<span data-ttu-id="24779-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24779-133">Here is a JSON representation of the resource.</span></span>
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



