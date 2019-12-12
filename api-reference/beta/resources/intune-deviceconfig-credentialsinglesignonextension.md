---
title: tipo de recurso credentialSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo de credencial.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9289416c33eaea89a24ffd01a1fb46026d1e7ef9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955698"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="47deb-103">tipo de recurso credentialSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="47deb-103">credentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="47deb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47deb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47deb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47deb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47deb-106">Representa um perfil de extensão de logon único de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="47deb-106">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="47deb-107">Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="47deb-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47deb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47deb-108">Properties</span></span>
|<span data-ttu-id="47deb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47deb-109">Property</span></span>|<span data-ttu-id="47deb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="47deb-110">Type</span></span>|<span data-ttu-id="47deb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="47deb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47deb-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="47deb-112">extensionIdentifier</span></span>|<span data-ttu-id="47deb-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="47deb-113">String</span></span>|<span data-ttu-id="47deb-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="47deb-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="47deb-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="47deb-115">teamIdentifier</span></span>|<span data-ttu-id="47deb-116">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="47deb-116">String</span></span>|<span data-ttu-id="47deb-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="47deb-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="47deb-118">domínio</span><span class="sxs-lookup"><span data-stu-id="47deb-118">domains</span></span>|<span data-ttu-id="47deb-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="47deb-119">String collection</span></span>|<span data-ttu-id="47deb-120">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="47deb-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="47deb-121">esfera</span><span class="sxs-lookup"><span data-stu-id="47deb-121">realm</span></span>|<span data-ttu-id="47deb-122">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="47deb-122">String</span></span>|<span data-ttu-id="47deb-123">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="47deb-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="47deb-124">as</span><span class="sxs-lookup"><span data-stu-id="47deb-124">configurations</span></span>|<span data-ttu-id="47deb-125">coleção [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="47deb-125">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="47deb-126">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="47deb-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="47deb-127">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="47deb-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47deb-128">Relações</span><span class="sxs-lookup"><span data-stu-id="47deb-128">Relationships</span></span>
<span data-ttu-id="47deb-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47deb-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47deb-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47deb-130">JSON Representation</span></span>
<span data-ttu-id="47deb-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47deb-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
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



