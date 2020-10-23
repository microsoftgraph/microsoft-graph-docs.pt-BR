---
title: tipo de recurso iosAzureAdSingleSignOnExtension
description: Representa um perfil de extensão single Sign-On de tipo de AD do Azure para dispositivos iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f330fad7553d702368c1b0f4a26eee0a35f40e32
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701533"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="3ecf4-103">tipo de recurso iosAzureAdSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="3ecf4-103">iosAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="3ecf4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ecf4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ecf4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ecf4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ecf4-107">Representa um perfil de extensão single Sign-On de tipo de AD do Azure para dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-107">Represents an Azure AD-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="3ecf4-108">Herda de [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="3ecf4-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ecf4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ecf4-109">Properties</span></span>
|<span data-ttu-id="3ecf4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ecf4-110">Property</span></span>|<span data-ttu-id="3ecf4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ecf4-111">Type</span></span>|<span data-ttu-id="3ecf4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ecf4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ecf4-113">enableSharedDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3ecf4-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="3ecf4-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ecf4-114">Boolean</span></span>|<span data-ttu-id="3ecf4-115">Habilita ou desabilita o modo de dispositivo compartilhado.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="3ecf4-116">bundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="3ecf4-116">bundleIdAccessControlList</span></span>|<span data-ttu-id="3ecf4-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ecf4-117">String collection</span></span>|<span data-ttu-id="3ecf4-118">Uma lista opcional de IDs de pacote adicionais que podem usar a extensão AAD para logon único.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-118">An optional list of additional bundle IDs allowed to use the AAD extension for single sign-on.</span></span>|
|<span data-ttu-id="3ecf4-119">as</span><span class="sxs-lookup"><span data-stu-id="3ecf4-119">configurations</span></span>|<span data-ttu-id="3ecf4-120">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3ecf4-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="3ecf4-121">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="3ecf4-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ecf4-123">Relações</span><span class="sxs-lookup"><span data-stu-id="3ecf4-123">Relationships</span></span>
<span data-ttu-id="3ecf4-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ecf4-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ecf4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ecf4-125">JSON Representation</span></span>
<span data-ttu-id="3ecf4-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ecf4-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```





