---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f17c22d8719f60ee28732727607db62422f1b74b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469243"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="d2060-103">tipo de recurso deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="d2060-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="d2060-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2060-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2060-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2060-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2060-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2060-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2060-107">Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2060-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="d2060-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2060-108">Properties</span></span>
|<span data-ttu-id="d2060-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2060-109">Property</span></span>|<span data-ttu-id="d2060-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2060-110">Type</span></span>|<span data-ttu-id="d2060-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2060-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2060-112">nome</span><span class="sxs-lookup"><span data-stu-id="d2060-112">name</span></span>|<span data-ttu-id="d2060-113">String</span><span class="sxs-lookup"><span data-stu-id="d2060-113">String</span></span>|<span data-ttu-id="d2060-114">O nome desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="d2060-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="d2060-115">description</span><span class="sxs-lookup"><span data-stu-id="d2060-115">description</span></span>|<span data-ttu-id="d2060-116">String</span><span class="sxs-lookup"><span data-stu-id="d2060-116">String</span></span>|<span data-ttu-id="d2060-117">Descrição do administrador desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="d2060-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="d2060-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d2060-118">securityIdentifier</span></span>|<span data-ttu-id="d2060-119">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d2060-119">String</span></span>|<span data-ttu-id="d2060-120">O identificador de segurança desse usuário ou grupo local (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="d2060-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2060-121">Relações</span><span class="sxs-lookup"><span data-stu-id="d2060-121">Relationships</span></span>
<span data-ttu-id="d2060-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2060-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2060-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2060-123">JSON Representation</span></span>
<span data-ttu-id="d2060-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2060-124">Here is a JSON representation of the resource.</span></span>
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



