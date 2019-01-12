---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b06e52d34cbbfb1e358ee2353c3420f8d129a61e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956931"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="12b6c-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="12b6c-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="12b6c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="12b6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12b6c-105">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="12b6c-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="12b6c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="12b6c-106">Methods</span></span>
|<span data-ttu-id="12b6c-107">Método</span><span class="sxs-lookup"><span data-stu-id="12b6c-107">Method</span></span>|<span data-ttu-id="12b6c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="12b6c-108">Return Type</span></span>|<span data-ttu-id="12b6c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="12b6c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12b6c-110">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="12b6c-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="12b6c-111">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="12b6c-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="12b6c-112">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="12b6c-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="12b6c-113">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="12b6c-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="12b6c-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="12b6c-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="12b6c-115">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="12b6c-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12b6c-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12b6c-116">Properties</span></span>
|<span data-ttu-id="12b6c-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12b6c-117">Property</span></span>|<span data-ttu-id="12b6c-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="12b6c-118">Type</span></span>|<span data-ttu-id="12b6c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="12b6c-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12b6c-120">displayName</span><span class="sxs-lookup"><span data-stu-id="12b6c-120">displayName</span></span>|<span data-ttu-id="12b6c-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12b6c-121">String</span></span>|<span data-ttu-id="12b6c-122">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="12b6c-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="12b6c-123">id</span><span class="sxs-lookup"><span data-stu-id="12b6c-123">id</span></span>|<span data-ttu-id="12b6c-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12b6c-124">String</span></span>|<span data-ttu-id="12b6c-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12b6c-125">Key of the entity.</span></span>|
|<span data-ttu-id="12b6c-126">version</span><span class="sxs-lookup"><span data-stu-id="12b6c-126">version</span></span>|<span data-ttu-id="12b6c-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12b6c-127">String</span></span>|<span data-ttu-id="12b6c-128">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="12b6c-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12b6c-129">Relações</span><span class="sxs-lookup"><span data-stu-id="12b6c-129">Relationships</span></span>
<span data-ttu-id="12b6c-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12b6c-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12b6c-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12b6c-131">JSON Representation</span></span>
<span data-ttu-id="12b6c-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12b6c-132">Here is a JSON representation of the resource.</span></span>
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



