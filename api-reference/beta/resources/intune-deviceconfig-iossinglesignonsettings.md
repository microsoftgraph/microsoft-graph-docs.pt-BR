---
title: tipo de recurso iosSingleSignOnSettings
description: configurações de autenticação Kerberos do iOS para logon único
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd959b3019a6bd4ce553b53a70042fffd5c9b277
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790535"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="ea25c-103">tipo de recurso iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="ea25c-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="ea25c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea25c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea25c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea25c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea25c-106">configurações de autenticação Kerberos do iOS para logon único</span><span class="sxs-lookup"><span data-stu-id="ea25c-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="ea25c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea25c-107">Properties</span></span>
|<span data-ttu-id="ea25c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea25c-108">Property</span></span>|<span data-ttu-id="ea25c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea25c-109">Type</span></span>|<span data-ttu-id="ea25c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea25c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea25c-111">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="ea25c-111">allowedAppsList</span></span>|<span data-ttu-id="ea25c-112">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea25c-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ea25c-113">Lista de identificadores de aplicativos que têm permissão para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="ea25c-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="ea25c-114">Se esse campo for omitido, o logon será aplicado a todos os aplicativos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea25c-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="ea25c-115">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ea25c-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ea25c-116">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="ea25c-116">allowedUrls</span></span>|<span data-ttu-id="ea25c-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea25c-117">String collection</span></span>|<span data-ttu-id="ea25c-118">Lista de URLs HTTP que devem ser correspondidas para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="ea25c-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="ea25c-119">Com o iOS 9,0 ou posterior, um caractere curinga pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="ea25c-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="ea25c-120">displayName</span><span class="sxs-lookup"><span data-stu-id="ea25c-120">displayName</span></span>|<span data-ttu-id="ea25c-121">String</span><span class="sxs-lookup"><span data-stu-id="ea25c-121">String</span></span>|<span data-ttu-id="ea25c-122">O nome de exibição das configurações de logon mostradas no dispositivo receptor.</span><span class="sxs-lookup"><span data-stu-id="ea25c-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="ea25c-123">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ea25c-123">kerberosPrincipalName</span></span>|<span data-ttu-id="ea25c-124">String</span><span class="sxs-lookup"><span data-stu-id="ea25c-124">String</span></span>|<span data-ttu-id="ea25c-125">Um nome principal Kerberos.</span><span class="sxs-lookup"><span data-stu-id="ea25c-125">A Kerberos principal name.</span></span> <span data-ttu-id="ea25c-126">Se não for fornecido, o usuário será solicitado a fornecer um durante a instalação do perfil.</span><span class="sxs-lookup"><span data-stu-id="ea25c-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="ea25c-127">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="ea25c-127">kerberosRealm</span></span>|<span data-ttu-id="ea25c-128">String</span><span class="sxs-lookup"><span data-stu-id="ea25c-128">String</span></span>|<span data-ttu-id="ea25c-129">Um nome de realm Kerberos.</span><span class="sxs-lookup"><span data-stu-id="ea25c-129">A Kerberos realm name.</span></span> <span data-ttu-id="ea25c-130">Diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ea25c-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea25c-131">Relações</span><span class="sxs-lookup"><span data-stu-id="ea25c-131">Relationships</span></span>
<span data-ttu-id="ea25c-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea25c-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea25c-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea25c-133">JSON Representation</span></span>
<span data-ttu-id="ea25c-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea25c-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```



