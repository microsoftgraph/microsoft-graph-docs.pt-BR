---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: tfitzmac
ms.openlocfilehash: e23b20b53d7ad89a4bbd0df8510a66e0f7da581d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331588"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="87955-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="87955-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="87955-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="87955-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87955-105">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="87955-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="87955-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="87955-106">Methods</span></span>
|<span data-ttu-id="87955-107">Método</span><span class="sxs-lookup"><span data-stu-id="87955-107">Method</span></span>|<span data-ttu-id="87955-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87955-108">Return Type</span></span>|<span data-ttu-id="87955-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="87955-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87955-110">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="87955-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="87955-111">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="87955-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="87955-112">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="87955-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="87955-113">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="87955-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="87955-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="87955-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="87955-115">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="87955-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87955-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87955-116">Properties</span></span>
|<span data-ttu-id="87955-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87955-117">Property</span></span>|<span data-ttu-id="87955-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="87955-118">Type</span></span>|<span data-ttu-id="87955-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="87955-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87955-120">displayName</span><span class="sxs-lookup"><span data-stu-id="87955-120">displayName</span></span>|<span data-ttu-id="87955-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87955-121">String</span></span>|<span data-ttu-id="87955-122">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="87955-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="87955-123">id</span><span class="sxs-lookup"><span data-stu-id="87955-123">id</span></span>|<span data-ttu-id="87955-124">String</span><span class="sxs-lookup"><span data-stu-id="87955-124">String</span></span>|<span data-ttu-id="87955-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87955-125">Key of the entity.</span></span>|
|<span data-ttu-id="87955-126">version</span><span class="sxs-lookup"><span data-stu-id="87955-126">version</span></span>|<span data-ttu-id="87955-127">String</span><span class="sxs-lookup"><span data-stu-id="87955-127">String</span></span>|<span data-ttu-id="87955-128">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="87955-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87955-129">Relações</span><span class="sxs-lookup"><span data-stu-id="87955-129">Relationships</span></span>
<span data-ttu-id="87955-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87955-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="87955-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87955-131">JSON Representation</span></span>
<span data-ttu-id="87955-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87955-132">Here is a JSON representation of the resource.</span></span>
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



