---
title: tipo de recurso loggedOnUser
description: Usuário conectado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a32ee6182f8937123662e3a8c3e4d18145607151
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372325"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="300d3-103">tipo de recurso loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="300d3-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="300d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="300d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="300d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="300d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="300d3-106">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="300d3-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="300d3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="300d3-107">Properties</span></span>
|<span data-ttu-id="300d3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="300d3-108">Property</span></span>|<span data-ttu-id="300d3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="300d3-109">Type</span></span>|<span data-ttu-id="300d3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="300d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="300d3-111">userId</span><span class="sxs-lookup"><span data-stu-id="300d3-111">userId</span></span>|<span data-ttu-id="300d3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="300d3-112">String</span></span>|<span data-ttu-id="300d3-113">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="300d3-113">User id</span></span>|
|<span data-ttu-id="300d3-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="300d3-114">lastLogOnDateTime</span></span>|<span data-ttu-id="300d3-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="300d3-115">DateTimeOffset</span></span>|<span data-ttu-id="300d3-116">Data e hora em que o usuário faz logon</span><span class="sxs-lookup"><span data-stu-id="300d3-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="300d3-117">Relações</span><span class="sxs-lookup"><span data-stu-id="300d3-117">Relationships</span></span>
<span data-ttu-id="300d3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="300d3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="300d3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="300d3-119">JSON Representation</span></span>
<span data-ttu-id="300d3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="300d3-120">Here is a JSON representation of the resource.</span></span>
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



