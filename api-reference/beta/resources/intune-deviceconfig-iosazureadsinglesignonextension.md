---
title: tipo de recurso iosAzureAdSingleSignOnExtension
description: Representa um perfil de extensão de logon único do Azure AD-Type para dispositivos iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9388b46457df2390a0820c1005f0df0e1cae9b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444203"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="1f9c3-103">tipo de recurso iosAzureAdSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="1f9c3-103">iosAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="1f9c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f9c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f9c3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f9c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f9c3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f9c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f9c3-107">Representa um perfil de extensão de logon único do Azure AD-Type para dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="1f9c3-107">Represents an Azure AD-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="1f9c3-108">Herda de [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="1f9c3-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f9c3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f9c3-109">Properties</span></span>
|<span data-ttu-id="1f9c3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f9c3-110">Property</span></span>|<span data-ttu-id="1f9c3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f9c3-111">Type</span></span>|<span data-ttu-id="1f9c3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f9c3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f9c3-113">enableSharedDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1f9c3-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="1f9c3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f9c3-114">Boolean</span></span>|<span data-ttu-id="1f9c3-115">Habilita ou desabilita o modo de dispositivo compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1f9c3-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="1f9c3-116">as</span><span class="sxs-lookup"><span data-stu-id="1f9c3-116">configurations</span></span>|<span data-ttu-id="1f9c3-117">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1f9c3-117">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="1f9c3-118">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="1f9c3-118">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="1f9c3-119">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1f9c3-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f9c3-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1f9c3-120">Relationships</span></span>
<span data-ttu-id="1f9c3-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f9c3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f9c3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f9c3-122">JSON Representation</span></span>
<span data-ttu-id="1f9c3-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f9c3-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```



