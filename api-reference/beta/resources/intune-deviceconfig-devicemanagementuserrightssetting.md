---
title: tipo de recurso de deviceManagementUserRightsSetting
description: Representa uma definição de direitos de usuário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35e6ec1a5faa5556a0e113df145d718c488b1669
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415051"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="26f63-103">tipo de recurso de deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="26f63-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="26f63-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="26f63-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="26f63-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26f63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26f63-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="26f63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26f63-107">Representa uma definição de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="26f63-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="26f63-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26f63-108">Properties</span></span>
|<span data-ttu-id="26f63-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26f63-109">Property</span></span>|<span data-ttu-id="26f63-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="26f63-110">Type</span></span>|<span data-ttu-id="26f63-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26f63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26f63-112">state</span><span class="sxs-lookup"><span data-stu-id="26f63-112">state</span></span>|[<span data-ttu-id="26f63-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="26f63-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="26f63-114">Configuração de direitos que representa o estado atual deste usuário.</span><span class="sxs-lookup"><span data-stu-id="26f63-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="26f63-115">Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="26f63-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="26f63-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="26f63-116">localUsersOrGroups</span></span>|<span data-ttu-id="26f63-117">coleção [deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="26f63-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="26f63-118">Que representa uma coleção de usuários ou grupos que serão definidos no dispositivo se o estado dessa configuração é permitido locais.</span><span class="sxs-lookup"><span data-stu-id="26f63-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="26f63-119">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="26f63-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26f63-120">Relações</span><span class="sxs-lookup"><span data-stu-id="26f63-120">Relationships</span></span>
<span data-ttu-id="26f63-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26f63-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26f63-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26f63-122">JSON Representation</span></span>
<span data-ttu-id="26f63-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26f63-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```




