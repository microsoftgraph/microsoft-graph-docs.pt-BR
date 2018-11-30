---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
ms.openlocfilehash: d25770468341e1f62e96273c6c925d322b385c89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005799"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="3c93e-103">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="3c93e-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="3c93e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c93e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c93e-105">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="3c93e-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="3c93e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3c93e-106">Methods</span></span>
|<span data-ttu-id="3c93e-107">Método</span><span class="sxs-lookup"><span data-stu-id="3c93e-107">Method</span></span>|<span data-ttu-id="3c93e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3c93e-108">Return Type</span></span>|<span data-ttu-id="3c93e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c93e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3c93e-110">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="3c93e-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="3c93e-111">Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="3c93e-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="3c93e-112">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3c93e-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="3c93e-113">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="3c93e-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="3c93e-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="3c93e-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="3c93e-115">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3c93e-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c93e-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c93e-116">Properties</span></span>
|<span data-ttu-id="3c93e-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c93e-117">Property</span></span>|<span data-ttu-id="3c93e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c93e-118">Type</span></span>|<span data-ttu-id="3c93e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c93e-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c93e-120">displayName</span><span class="sxs-lookup"><span data-stu-id="3c93e-120">displayName</span></span>|<span data-ttu-id="3c93e-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c93e-121">String</span></span>|<span data-ttu-id="3c93e-122">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="3c93e-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="3c93e-123">id</span><span class="sxs-lookup"><span data-stu-id="3c93e-123">id</span></span>|<span data-ttu-id="3c93e-124">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-124">String</span></span>|<span data-ttu-id="3c93e-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c93e-125">Key of the entity.</span></span>|
|<span data-ttu-id="3c93e-126">version</span><span class="sxs-lookup"><span data-stu-id="3c93e-126">version</span></span>|<span data-ttu-id="3c93e-127">String</span><span class="sxs-lookup"><span data-stu-id="3c93e-127">String</span></span>|<span data-ttu-id="3c93e-128">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c93e-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c93e-129">Relações</span><span class="sxs-lookup"><span data-stu-id="3c93e-129">Relationships</span></span>
<span data-ttu-id="3c93e-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c93e-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c93e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c93e-131">JSON Representation</span></span>
<span data-ttu-id="3c93e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c93e-132">Here is a JSON representation of the resource.</span></span>
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



