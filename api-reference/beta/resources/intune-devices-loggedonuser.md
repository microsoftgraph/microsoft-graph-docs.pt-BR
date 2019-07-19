---
title: tipo de recurso loggedOnUser
description: Usuário conectado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e013b89eefbcdb1bf180ff90341388db9c05dcf4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995151"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="1df22-103">tipo de recurso loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="1df22-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="1df22-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1df22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1df22-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1df22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1df22-106">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="1df22-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="1df22-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1df22-107">Properties</span></span>
|<span data-ttu-id="1df22-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1df22-108">Property</span></span>|<span data-ttu-id="1df22-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1df22-109">Type</span></span>|<span data-ttu-id="1df22-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1df22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df22-111">userId</span><span class="sxs-lookup"><span data-stu-id="1df22-111">userId</span></span>|<span data-ttu-id="1df22-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1df22-112">String</span></span>|<span data-ttu-id="1df22-113">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="1df22-113">User id</span></span>|
|<span data-ttu-id="1df22-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="1df22-114">lastLogOnDateTime</span></span>|<span data-ttu-id="1df22-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1df22-115">DateTimeOffset</span></span>|<span data-ttu-id="1df22-116">Data e hora em que o usuário faz logon</span><span class="sxs-lookup"><span data-stu-id="1df22-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="1df22-117">Relações</span><span class="sxs-lookup"><span data-stu-id="1df22-117">Relationships</span></span>
<span data-ttu-id="1df22-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1df22-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1df22-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1df22-119">JSON Representation</span></span>
<span data-ttu-id="1df22-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1df22-120">Here is a JSON representation of the resource.</span></span>
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





