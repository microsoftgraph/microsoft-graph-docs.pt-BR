---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6df9c36f15e3e20389dfc46d306b896c3fe77b5b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551726"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="87a85-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="87a85-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="87a85-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87a85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87a85-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87a85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a85-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="87a85-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="87a85-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="87a85-107">Methods</span></span>
|<span data-ttu-id="87a85-108">Método</span><span class="sxs-lookup"><span data-stu-id="87a85-108">Method</span></span>|<span data-ttu-id="87a85-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87a85-109">Return Type</span></span>|<span data-ttu-id="87a85-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a85-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87a85-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="87a85-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="87a85-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="87a85-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="87a85-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="87a85-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="87a85-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="87a85-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="87a85-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="87a85-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="87a85-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="87a85-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87a85-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87a85-117">Properties</span></span>
|<span data-ttu-id="87a85-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87a85-118">Property</span></span>|<span data-ttu-id="87a85-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="87a85-119">Type</span></span>|<span data-ttu-id="87a85-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a85-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a85-121">displayName</span><span class="sxs-lookup"><span data-stu-id="87a85-121">displayName</span></span>|<span data-ttu-id="87a85-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a85-122">String</span></span>|<span data-ttu-id="87a85-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="87a85-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="87a85-124">id</span><span class="sxs-lookup"><span data-stu-id="87a85-124">id</span></span>|<span data-ttu-id="87a85-125">String</span><span class="sxs-lookup"><span data-stu-id="87a85-125">String</span></span>|<span data-ttu-id="87a85-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87a85-126">Key of the entity.</span></span>|
|<span data-ttu-id="87a85-127">versão</span><span class="sxs-lookup"><span data-stu-id="87a85-127">version</span></span>|<span data-ttu-id="87a85-128">String</span><span class="sxs-lookup"><span data-stu-id="87a85-128">String</span></span>|<span data-ttu-id="87a85-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="87a85-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87a85-130">Relações</span><span class="sxs-lookup"><span data-stu-id="87a85-130">Relationships</span></span>
<span data-ttu-id="87a85-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87a85-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87a85-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87a85-132">JSON Representation</span></span>
<span data-ttu-id="87a85-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87a85-133">Here is a JSON representation of the resource.</span></span>
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





