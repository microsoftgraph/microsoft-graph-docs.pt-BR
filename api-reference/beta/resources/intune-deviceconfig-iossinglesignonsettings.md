---
title: tipo de recurso iosSingleSignOnSettings
description: configurações de autenticação Kerberos do iOS para logon único
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20c6cabbd5f18349058c68136052c8d56894dccc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728560"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="ff832-103">tipo de recurso iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="ff832-103">iosSingleSignOnSettings resource type</span></span>

<span data-ttu-id="ff832-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff832-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff832-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff832-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff832-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff832-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff832-107">configurações de autenticação Kerberos do iOS para logon único</span><span class="sxs-lookup"><span data-stu-id="ff832-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="ff832-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff832-108">Properties</span></span>
|<span data-ttu-id="ff832-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff832-109">Property</span></span>|<span data-ttu-id="ff832-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff832-110">Type</span></span>|<span data-ttu-id="ff832-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff832-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff832-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="ff832-112">allowedAppsList</span></span>|<span data-ttu-id="ff832-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ff832-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ff832-114">Lista de identificadores de aplicativos que têm permissão para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="ff832-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="ff832-115">Se esse campo for omitido, o logon será aplicado a todos os aplicativos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff832-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="ff832-116">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ff832-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ff832-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="ff832-117">allowedUrls</span></span>|<span data-ttu-id="ff832-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff832-118">String collection</span></span>|<span data-ttu-id="ff832-119">Lista de URLs HTTP que devem ser correspondidas para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="ff832-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="ff832-120">Com o iOS 9,0 ou posterior, um caractere curinga pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="ff832-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="ff832-121">displayName</span><span class="sxs-lookup"><span data-stu-id="ff832-121">displayName</span></span>|<span data-ttu-id="ff832-122">String</span><span class="sxs-lookup"><span data-stu-id="ff832-122">String</span></span>|<span data-ttu-id="ff832-123">O nome de exibição das configurações de logon mostradas no dispositivo receptor.</span><span class="sxs-lookup"><span data-stu-id="ff832-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="ff832-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ff832-124">kerberosPrincipalName</span></span>|<span data-ttu-id="ff832-125">String</span><span class="sxs-lookup"><span data-stu-id="ff832-125">String</span></span>|<span data-ttu-id="ff832-126">Um nome principal Kerberos.</span><span class="sxs-lookup"><span data-stu-id="ff832-126">A Kerberos principal name.</span></span> <span data-ttu-id="ff832-127">Se não for fornecido, o usuário será solicitado a fornecer um durante a instalação do perfil.</span><span class="sxs-lookup"><span data-stu-id="ff832-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="ff832-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="ff832-128">kerberosRealm</span></span>|<span data-ttu-id="ff832-129">String</span><span class="sxs-lookup"><span data-stu-id="ff832-129">String</span></span>|<span data-ttu-id="ff832-130">Um nome de realm Kerberos.</span><span class="sxs-lookup"><span data-stu-id="ff832-130">A Kerberos realm name.</span></span> <span data-ttu-id="ff832-131">Diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ff832-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff832-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ff832-132">Relationships</span></span>
<span data-ttu-id="ff832-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff832-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff832-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff832-134">JSON Representation</span></span>
<span data-ttu-id="ff832-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff832-135">Here is a JSON representation of the resource.</span></span>
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





