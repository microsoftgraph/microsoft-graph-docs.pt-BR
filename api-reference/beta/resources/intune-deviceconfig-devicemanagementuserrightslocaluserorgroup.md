---
title: tipo de recurso de deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
ms.openlocfilehash: bf81a36a8e102bea4c3e8fb56e45bf7822cf31a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037305"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="71eb0-103">tipo de recurso de deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="71eb0-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="71eb0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="71eb0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71eb0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="71eb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71eb0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71eb0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71eb0-107">Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="71eb0-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="71eb0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71eb0-108">Properties</span></span>
|<span data-ttu-id="71eb0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71eb0-109">Property</span></span>|<span data-ttu-id="71eb0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="71eb0-110">Type</span></span>|<span data-ttu-id="71eb0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71eb0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71eb0-112">name</span><span class="sxs-lookup"><span data-stu-id="71eb0-112">name</span></span>|<span data-ttu-id="71eb0-113">String</span><span class="sxs-lookup"><span data-stu-id="71eb0-113">String</span></span>|<span data-ttu-id="71eb0-114">O nome deste usuário local ou grupo.</span><span class="sxs-lookup"><span data-stu-id="71eb0-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="71eb0-115">description</span><span class="sxs-lookup"><span data-stu-id="71eb0-115">description</span></span>|<span data-ttu-id="71eb0-116">String</span><span class="sxs-lookup"><span data-stu-id="71eb0-116">String</span></span>|<span data-ttu-id="71eb0-117">Descrição do Admin este usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="71eb0-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="71eb0-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="71eb0-118">securityIdentifier</span></span>|<span data-ttu-id="71eb0-119">String</span><span class="sxs-lookup"><span data-stu-id="71eb0-119">String</span></span>|<span data-ttu-id="71eb0-120">O identificador de segurança deste usuário local ou grupo (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="71eb0-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="71eb0-121">Relações</span><span class="sxs-lookup"><span data-stu-id="71eb0-121">Relationships</span></span>
<span data-ttu-id="71eb0-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71eb0-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71eb0-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71eb0-123">JSON Representation</span></span>
<span data-ttu-id="71eb0-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71eb0-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





