---
title: tipo de recurso de loggedOnUser
description: Usuário conectado
ms.openlocfilehash: 37df6b5343df515a76bc6b755889156cb86c4bf0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040937"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="050b6-103">tipo de recurso de loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="050b6-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="050b6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="050b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="050b6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="050b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="050b6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="050b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="050b6-107">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="050b6-107">Logged On User</span></span>
## <a name="properties"></a><span data-ttu-id="050b6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="050b6-108">Properties</span></span>
|<span data-ttu-id="050b6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="050b6-109">Property</span></span>|<span data-ttu-id="050b6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="050b6-110">Type</span></span>|<span data-ttu-id="050b6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="050b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="050b6-112">userId</span><span class="sxs-lookup"><span data-stu-id="050b6-112">userId</span></span>|<span data-ttu-id="050b6-113">String</span><span class="sxs-lookup"><span data-stu-id="050b6-113">String</span></span>|<span data-ttu-id="050b6-114">Id de usuário</span><span class="sxs-lookup"><span data-stu-id="050b6-114">User id</span></span>|
|<span data-ttu-id="050b6-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="050b6-115">lastLogOnDateTime</span></span>|<span data-ttu-id="050b6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050b6-116">DateTimeOffset</span></span>|<span data-ttu-id="050b6-117">Data e hora de quando o usuário fizer logon</span><span class="sxs-lookup"><span data-stu-id="050b6-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="050b6-118">Relações</span><span class="sxs-lookup"><span data-stu-id="050b6-118">Relationships</span></span>
<span data-ttu-id="050b6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="050b6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="050b6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="050b6-120">JSON Representation</span></span>
<span data-ttu-id="050b6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="050b6-121">Here is a JSON representation of the resource.</span></span>
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





