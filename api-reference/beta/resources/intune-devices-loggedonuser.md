---
title: tipo de recurso loggedOnUser
description: Usuário conectado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2b92d8504ba4854109efa30d0637bca1ea35d7b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799458"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="8781a-103">tipo de recurso loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="8781a-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="8781a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8781a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8781a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8781a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8781a-106">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="8781a-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="8781a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8781a-107">Properties</span></span>
|<span data-ttu-id="8781a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8781a-108">Property</span></span>|<span data-ttu-id="8781a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8781a-109">Type</span></span>|<span data-ttu-id="8781a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8781a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8781a-111">userId</span><span class="sxs-lookup"><span data-stu-id="8781a-111">userId</span></span>|<span data-ttu-id="8781a-112">String</span><span class="sxs-lookup"><span data-stu-id="8781a-112">String</span></span>|<span data-ttu-id="8781a-113">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="8781a-113">User id</span></span>|
|<span data-ttu-id="8781a-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="8781a-114">lastLogOnDateTime</span></span>|<span data-ttu-id="8781a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8781a-115">DateTimeOffset</span></span>|<span data-ttu-id="8781a-116">Data e hora em que o usuário faz logon</span><span class="sxs-lookup"><span data-stu-id="8781a-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="8781a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8781a-117">Relationships</span></span>
<span data-ttu-id="8781a-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8781a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8781a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8781a-119">JSON Representation</span></span>
<span data-ttu-id="8781a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8781a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```





