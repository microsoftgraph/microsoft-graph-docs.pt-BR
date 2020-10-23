---
title: tipo de recurso macOSAzureAdSingleSignOnExtension
description: Representa um perfil de extensão single Sign-On de tipo de AD do Azure para dispositivos macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bc80bb752230fd1699091c380538e62d4ca09c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736244"
---
# <a name="macosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="990b3-103">tipo de recurso macOSAzureAdSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="990b3-103">macOSAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="990b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="990b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="990b3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="990b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="990b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="990b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="990b3-107">Representa um perfil de extensão single Sign-On de tipo de AD do Azure para dispositivos macOS.</span><span class="sxs-lookup"><span data-stu-id="990b3-107">Represents an Azure AD-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="990b3-108">Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="990b3-108">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="990b3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="990b3-109">Properties</span></span>
|<span data-ttu-id="990b3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="990b3-110">Property</span></span>|<span data-ttu-id="990b3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="990b3-111">Type</span></span>|<span data-ttu-id="990b3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="990b3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="990b3-113">enableSharedDeviceMode</span><span class="sxs-lookup"><span data-stu-id="990b3-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="990b3-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="990b3-114">Boolean</span></span>|<span data-ttu-id="990b3-115">Habilita ou desabilita o modo de dispositivo compartilhado.</span><span class="sxs-lookup"><span data-stu-id="990b3-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="990b3-116">bundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="990b3-116">bundleIdAccessControlList</span></span>|<span data-ttu-id="990b3-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="990b3-117">String collection</span></span>|<span data-ttu-id="990b3-118">Uma lista opcional de IDs de pacote adicionais que podem usar a extensão AAD para logon único.</span><span class="sxs-lookup"><span data-stu-id="990b3-118">An optional list of additional bundle IDs allowed to use the AAD extension for single sign-on.</span></span>|
|<span data-ttu-id="990b3-119">as</span><span class="sxs-lookup"><span data-stu-id="990b3-119">configurations</span></span>|<span data-ttu-id="990b3-120">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="990b3-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="990b3-121">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="990b3-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="990b3-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="990b3-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="990b3-123">Relações</span><span class="sxs-lookup"><span data-stu-id="990b3-123">Relationships</span></span>
<span data-ttu-id="990b3-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="990b3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="990b3-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="990b3-125">JSON Representation</span></span>
<span data-ttu-id="990b3-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="990b3-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```





