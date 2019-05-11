---
title: tipo de recurso loggedOnUser
description: Usuário conectado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeacee7d4d3a22e0d069851c1f9271ceb0e32c0d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941965"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="53f65-103">tipo de recurso loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="53f65-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="53f65-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53f65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53f65-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53f65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53f65-106">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="53f65-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="53f65-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53f65-107">Properties</span></span>
|<span data-ttu-id="53f65-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53f65-108">Property</span></span>|<span data-ttu-id="53f65-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="53f65-109">Type</span></span>|<span data-ttu-id="53f65-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="53f65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53f65-111">userId</span><span class="sxs-lookup"><span data-stu-id="53f65-111">userId</span></span>|<span data-ttu-id="53f65-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53f65-112">String</span></span>|<span data-ttu-id="53f65-113">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="53f65-113">User id</span></span>|
|<span data-ttu-id="53f65-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="53f65-114">lastLogOnDateTime</span></span>|<span data-ttu-id="53f65-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53f65-115">DateTimeOffset</span></span>|<span data-ttu-id="53f65-116">Data e hora em que o usuário faz logon</span><span class="sxs-lookup"><span data-stu-id="53f65-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="53f65-117">Relações</span><span class="sxs-lookup"><span data-stu-id="53f65-117">Relationships</span></span>
<span data-ttu-id="53f65-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53f65-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53f65-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53f65-119">JSON Representation</span></span>
<span data-ttu-id="53f65-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53f65-120">Here is a JSON representation of the resource.</span></span>
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




