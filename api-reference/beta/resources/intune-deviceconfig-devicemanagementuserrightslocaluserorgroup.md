---
title: tipo de recurso de deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a2cc0ff5b9e054398e7878b7d99619b59d109a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422058"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="cbcf0-103">tipo de recurso de deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="cbcf0-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="cbcf0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cbcf0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cbcf0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cbcf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbcf0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cbcf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbcf0-107">Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="cbcf0-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="cbcf0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbcf0-108">Properties</span></span>
|<span data-ttu-id="cbcf0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbcf0-109">Property</span></span>|<span data-ttu-id="cbcf0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbcf0-110">Type</span></span>|<span data-ttu-id="cbcf0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbcf0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbcf0-112">name</span><span class="sxs-lookup"><span data-stu-id="cbcf0-112">name</span></span>|<span data-ttu-id="cbcf0-113">String</span><span class="sxs-lookup"><span data-stu-id="cbcf0-113">String</span></span>|<span data-ttu-id="cbcf0-114">O nome deste usuário local ou grupo.</span><span class="sxs-lookup"><span data-stu-id="cbcf0-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="cbcf0-115">description</span><span class="sxs-lookup"><span data-stu-id="cbcf0-115">description</span></span>|<span data-ttu-id="cbcf0-116">String</span><span class="sxs-lookup"><span data-stu-id="cbcf0-116">String</span></span>|<span data-ttu-id="cbcf0-117">Descrição do Admin este usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="cbcf0-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="cbcf0-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="cbcf0-118">securityIdentifier</span></span>|<span data-ttu-id="cbcf0-119">String</span><span class="sxs-lookup"><span data-stu-id="cbcf0-119">String</span></span>|<span data-ttu-id="cbcf0-120">O identificador de segurança deste usuário local ou grupo (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="cbcf0-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbcf0-121">Relações</span><span class="sxs-lookup"><span data-stu-id="cbcf0-121">Relationships</span></span>
<span data-ttu-id="cbcf0-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbcf0-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbcf0-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbcf0-123">JSON Representation</span></span>
<span data-ttu-id="cbcf0-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbcf0-124">Here is a JSON representation of the resource.</span></span>
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




