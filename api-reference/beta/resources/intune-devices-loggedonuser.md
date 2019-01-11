---
title: tipo de recurso de loggedOnUser
description: Usuário conectado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e832c6452b73a6fad39723675acb129d79c2b888
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859749"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="86764-103">tipo de recurso de loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="86764-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="86764-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="86764-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86764-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="86764-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86764-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="86764-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86764-107">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="86764-107">Logged On User</span></span>
## <a name="properties"></a><span data-ttu-id="86764-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86764-108">Properties</span></span>
|<span data-ttu-id="86764-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86764-109">Property</span></span>|<span data-ttu-id="86764-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="86764-110">Type</span></span>|<span data-ttu-id="86764-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86764-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86764-112">userId</span><span class="sxs-lookup"><span data-stu-id="86764-112">userId</span></span>|<span data-ttu-id="86764-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86764-113">String</span></span>|<span data-ttu-id="86764-114">Id de usuário</span><span class="sxs-lookup"><span data-stu-id="86764-114">User id</span></span>|
|<span data-ttu-id="86764-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="86764-115">lastLogOnDateTime</span></span>|<span data-ttu-id="86764-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86764-116">DateTimeOffset</span></span>|<span data-ttu-id="86764-117">Data e hora de quando o usuário fizer logon</span><span class="sxs-lookup"><span data-stu-id="86764-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="86764-118">Relações</span><span class="sxs-lookup"><span data-stu-id="86764-118">Relationships</span></span>
<span data-ttu-id="86764-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86764-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="86764-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86764-120">JSON Representation</span></span>
<span data-ttu-id="86764-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86764-121">Here is a JSON representation of the resource.</span></span>
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





