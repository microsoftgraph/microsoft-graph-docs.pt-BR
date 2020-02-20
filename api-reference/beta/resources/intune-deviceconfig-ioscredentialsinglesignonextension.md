---
title: tipo de recurso iosCredentialSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo de credencial para dispositivos iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a22b01e4429658e712e8bc98123d56d61621b23
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163840"
---
# <a name="ioscredentialsinglesignonextension-resource-type"></a><span data-ttu-id="0e336-103">tipo de recurso iosCredentialSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="0e336-103">iosCredentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="0e336-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e336-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e336-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e336-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e336-106">Representa um perfil de extensão de logon único de tipo de credencial para dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="0e336-106">Represents a Credential-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="0e336-107">Herda de [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="0e336-107">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0e336-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e336-108">Properties</span></span>
|<span data-ttu-id="0e336-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e336-109">Property</span></span>|<span data-ttu-id="0e336-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e336-110">Type</span></span>|<span data-ttu-id="0e336-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e336-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e336-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="0e336-112">extensionIdentifier</span></span>|<span data-ttu-id="0e336-113">String</span><span class="sxs-lookup"><span data-stu-id="0e336-113">String</span></span>|<span data-ttu-id="0e336-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="0e336-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="0e336-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="0e336-115">teamIdentifier</span></span>|<span data-ttu-id="0e336-116">String</span><span class="sxs-lookup"><span data-stu-id="0e336-116">String</span></span>|<span data-ttu-id="0e336-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="0e336-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="0e336-118">domínio</span><span class="sxs-lookup"><span data-stu-id="0e336-118">domains</span></span>|<span data-ttu-id="0e336-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e336-119">String collection</span></span>|<span data-ttu-id="0e336-120">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="0e336-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="0e336-121">esfera</span><span class="sxs-lookup"><span data-stu-id="0e336-121">realm</span></span>|<span data-ttu-id="0e336-122">String</span><span class="sxs-lookup"><span data-stu-id="0e336-122">String</span></span>|<span data-ttu-id="0e336-123">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="0e336-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="0e336-124">as</span><span class="sxs-lookup"><span data-stu-id="0e336-124">configurations</span></span>|<span data-ttu-id="0e336-125">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0e336-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="0e336-126">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="0e336-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="0e336-127">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0e336-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e336-128">Relações</span><span class="sxs-lookup"><span data-stu-id="0e336-128">Relationships</span></span>
<span data-ttu-id="0e336-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e336-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e336-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e336-130">JSON Representation</span></span>
<span data-ttu-id="0e336-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e336-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCredentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```



