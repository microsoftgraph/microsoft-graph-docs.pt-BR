---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca78f4dd9a191819e7f5e74ecea491ce7ceb7ec2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354286"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="0f776-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0f776-103">managedAppStatus resource type</span></span>

<span data-ttu-id="0f776-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f776-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f776-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f776-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f776-106">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="0f776-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="0f776-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0f776-107">Methods</span></span>
|<span data-ttu-id="0f776-108">Método</span><span class="sxs-lookup"><span data-stu-id="0f776-108">Method</span></span>|<span data-ttu-id="0f776-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f776-109">Return Type</span></span>|<span data-ttu-id="0f776-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f776-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f776-111">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="0f776-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="0f776-112">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f776-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="0f776-113">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0f776-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="0f776-114">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0f776-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="0f776-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0f776-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="0f776-116">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0f776-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f776-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f776-117">Properties</span></span>
|<span data-ttu-id="0f776-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f776-118">Property</span></span>|<span data-ttu-id="0f776-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f776-119">Type</span></span>|<span data-ttu-id="0f776-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f776-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f776-121">displayName</span><span class="sxs-lookup"><span data-stu-id="0f776-121">displayName</span></span>|<span data-ttu-id="0f776-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f776-122">String</span></span>|<span data-ttu-id="0f776-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="0f776-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="0f776-124">id</span><span class="sxs-lookup"><span data-stu-id="0f776-124">id</span></span>|<span data-ttu-id="0f776-125">String</span><span class="sxs-lookup"><span data-stu-id="0f776-125">String</span></span>|<span data-ttu-id="0f776-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f776-126">Key of the entity.</span></span>|
|<span data-ttu-id="0f776-127">versão</span><span class="sxs-lookup"><span data-stu-id="0f776-127">version</span></span>|<span data-ttu-id="0f776-128">String</span><span class="sxs-lookup"><span data-stu-id="0f776-128">String</span></span>|<span data-ttu-id="0f776-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f776-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f776-130">Relações</span><span class="sxs-lookup"><span data-stu-id="0f776-130">Relationships</span></span>
<span data-ttu-id="0f776-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f776-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f776-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f776-132">JSON Representation</span></span>
<span data-ttu-id="0f776-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f776-133">Here is a JSON representation of the resource.</span></span>
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







