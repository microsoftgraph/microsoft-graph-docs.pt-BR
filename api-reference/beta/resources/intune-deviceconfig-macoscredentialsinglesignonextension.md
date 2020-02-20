---
title: tipo de recurso macOSCredentialSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo de credencial para dispositivos macOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 226f9bc0ec559bad7ba155aff6da864525882822
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163469"
---
# <a name="macoscredentialsinglesignonextension-resource-type"></a><span data-ttu-id="96c77-103">tipo de recurso macOSCredentialSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="96c77-103">macOSCredentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="96c77-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96c77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96c77-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96c77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96c77-106">Representa um perfil de extensão de logon único de tipo de credencial para dispositivos macOS.</span><span class="sxs-lookup"><span data-stu-id="96c77-106">Represents a Credential-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="96c77-107">Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="96c77-107">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96c77-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96c77-108">Properties</span></span>
|<span data-ttu-id="96c77-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96c77-109">Property</span></span>|<span data-ttu-id="96c77-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="96c77-110">Type</span></span>|<span data-ttu-id="96c77-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96c77-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="96c77-112">extensionIdentifier</span></span>|<span data-ttu-id="96c77-113">String</span><span class="sxs-lookup"><span data-stu-id="96c77-113">String</span></span>|<span data-ttu-id="96c77-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="96c77-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="96c77-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="96c77-115">teamIdentifier</span></span>|<span data-ttu-id="96c77-116">String</span><span class="sxs-lookup"><span data-stu-id="96c77-116">String</span></span>|<span data-ttu-id="96c77-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="96c77-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="96c77-118">domínio</span><span class="sxs-lookup"><span data-stu-id="96c77-118">domains</span></span>|<span data-ttu-id="96c77-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="96c77-119">String collection</span></span>|<span data-ttu-id="96c77-120">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="96c77-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="96c77-121">esfera</span><span class="sxs-lookup"><span data-stu-id="96c77-121">realm</span></span>|<span data-ttu-id="96c77-122">String</span><span class="sxs-lookup"><span data-stu-id="96c77-122">String</span></span>|<span data-ttu-id="96c77-123">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="96c77-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="96c77-124">as</span><span class="sxs-lookup"><span data-stu-id="96c77-124">configurations</span></span>|<span data-ttu-id="96c77-125">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="96c77-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="96c77-126">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="96c77-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="96c77-127">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="96c77-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96c77-128">Relações</span><span class="sxs-lookup"><span data-stu-id="96c77-128">Relationships</span></span>
<span data-ttu-id="96c77-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96c77-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96c77-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96c77-130">JSON Representation</span></span>
<span data-ttu-id="96c77-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96c77-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCredentialSingleSignOnExtension",
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



