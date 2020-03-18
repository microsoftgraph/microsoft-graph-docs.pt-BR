---
title: tipo de recurso loggedOnUser
description: Usuário conectado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cab517ec064cea375efd8effaca9d31159e64bcd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783988"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="c137b-103">tipo de recurso loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="c137b-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="c137b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c137b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c137b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c137b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c137b-106">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="c137b-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="c137b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c137b-107">Properties</span></span>
|<span data-ttu-id="c137b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c137b-108">Property</span></span>|<span data-ttu-id="c137b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c137b-109">Type</span></span>|<span data-ttu-id="c137b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c137b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c137b-111">userId</span><span class="sxs-lookup"><span data-stu-id="c137b-111">userId</span></span>|<span data-ttu-id="c137b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c137b-112">String</span></span>|<span data-ttu-id="c137b-113">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="c137b-113">User id</span></span>|
|<span data-ttu-id="c137b-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="c137b-114">lastLogOnDateTime</span></span>|<span data-ttu-id="c137b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c137b-115">DateTimeOffset</span></span>|<span data-ttu-id="c137b-116">Data e hora em que o usuário faz logon</span><span class="sxs-lookup"><span data-stu-id="c137b-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="c137b-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c137b-117">Relationships</span></span>
<span data-ttu-id="c137b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c137b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c137b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c137b-119">JSON Representation</span></span>
<span data-ttu-id="c137b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c137b-120">Here is a JSON representation of the resource.</span></span>
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



