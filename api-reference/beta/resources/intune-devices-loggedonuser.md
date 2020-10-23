---
title: tipo de recurso loggedOnUser
description: Usuário conectado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c37ca746a2adc1ea1cba92839bce3903f947e4d6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729303"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="f44e1-103">tipo de recurso loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="f44e1-103">loggedOnUser resource type</span></span>

<span data-ttu-id="f44e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f44e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f44e1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f44e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f44e1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f44e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f44e1-107">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="f44e1-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="f44e1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f44e1-108">Properties</span></span>
|<span data-ttu-id="f44e1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f44e1-109">Property</span></span>|<span data-ttu-id="f44e1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f44e1-110">Type</span></span>|<span data-ttu-id="f44e1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f44e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f44e1-112">userId</span><span class="sxs-lookup"><span data-stu-id="f44e1-112">userId</span></span>|<span data-ttu-id="f44e1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f44e1-113">String</span></span>|<span data-ttu-id="f44e1-114">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="f44e1-114">User id</span></span>|
|<span data-ttu-id="f44e1-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="f44e1-115">lastLogOnDateTime</span></span>|<span data-ttu-id="f44e1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f44e1-116">DateTimeOffset</span></span>|<span data-ttu-id="f44e1-117">Data e hora em que o usuário faz logon</span><span class="sxs-lookup"><span data-stu-id="f44e1-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="f44e1-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f44e1-118">Relationships</span></span>
<span data-ttu-id="f44e1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f44e1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f44e1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f44e1-120">JSON Representation</span></span>
<span data-ttu-id="f44e1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f44e1-121">Here is a JSON representation of the resource.</span></span>
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





