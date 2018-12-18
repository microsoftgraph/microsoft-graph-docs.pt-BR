---
title: tipo de recurso de deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303728"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="17318-103">tipo de recurso de deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="17318-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="17318-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17318-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17318-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17318-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17318-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="17318-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17318-107">Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="17318-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="17318-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17318-108">Properties</span></span>
|<span data-ttu-id="17318-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17318-109">Property</span></span>|<span data-ttu-id="17318-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="17318-110">Type</span></span>|<span data-ttu-id="17318-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="17318-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17318-112">name</span><span class="sxs-lookup"><span data-stu-id="17318-112">name</span></span>|<span data-ttu-id="17318-113">String</span><span class="sxs-lookup"><span data-stu-id="17318-113">String</span></span>|<span data-ttu-id="17318-114">O nome deste usuário local ou grupo.</span><span class="sxs-lookup"><span data-stu-id="17318-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="17318-115">description</span><span class="sxs-lookup"><span data-stu-id="17318-115">description</span></span>|<span data-ttu-id="17318-116">String</span><span class="sxs-lookup"><span data-stu-id="17318-116">String</span></span>|<span data-ttu-id="17318-117">Descrição do Admin este usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="17318-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="17318-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="17318-118">securityIdentifier</span></span>|<span data-ttu-id="17318-119">String</span><span class="sxs-lookup"><span data-stu-id="17318-119">String</span></span>|<span data-ttu-id="17318-120">O identificador de segurança deste usuário local ou grupo (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="17318-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="17318-121">Relações</span><span class="sxs-lookup"><span data-stu-id="17318-121">Relationships</span></span>
<span data-ttu-id="17318-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17318-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17318-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17318-123">JSON Representation</span></span>
<span data-ttu-id="17318-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17318-124">Here is a JSON representation of the resource.</span></span>
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





