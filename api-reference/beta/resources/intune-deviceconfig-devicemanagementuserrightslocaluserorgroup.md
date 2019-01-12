---
title: tipo de recurso de deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 63e2dc3d16d17b76c4437e76eae642976711071c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972891"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="c4e39-103">tipo de recurso de deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="c4e39-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="c4e39-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c4e39-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4e39-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c4e39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4e39-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c4e39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4e39-107">Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="c4e39-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="c4e39-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4e39-108">Properties</span></span>
|<span data-ttu-id="c4e39-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4e39-109">Property</span></span>|<span data-ttu-id="c4e39-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4e39-110">Type</span></span>|<span data-ttu-id="c4e39-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4e39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4e39-112">name</span><span class="sxs-lookup"><span data-stu-id="c4e39-112">name</span></span>|<span data-ttu-id="c4e39-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4e39-113">String</span></span>|<span data-ttu-id="c4e39-114">O nome deste usuário local ou grupo.</span><span class="sxs-lookup"><span data-stu-id="c4e39-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="c4e39-115">description</span><span class="sxs-lookup"><span data-stu-id="c4e39-115">description</span></span>|<span data-ttu-id="c4e39-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4e39-116">String</span></span>|<span data-ttu-id="c4e39-117">Descrição do Admin este usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="c4e39-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="c4e39-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="c4e39-118">securityIdentifier</span></span>|<span data-ttu-id="c4e39-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4e39-119">String</span></span>|<span data-ttu-id="c4e39-120">O identificador de segurança deste usuário local ou grupo (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="c4e39-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4e39-121">Relações</span><span class="sxs-lookup"><span data-stu-id="c4e39-121">Relationships</span></span>
<span data-ttu-id="c4e39-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c4e39-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4e39-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4e39-123">JSON Representation</span></span>
<span data-ttu-id="c4e39-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4e39-124">Here is a JSON representation of the resource.</span></span>
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





