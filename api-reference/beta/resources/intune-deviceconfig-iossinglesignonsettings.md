---
title: tipo de recurso iosSingleSignOnSettings
description: configurações de autenticação Kerberos do iOS para logon único
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b438ea8fadc30a0bf5fa3786e9b4cec3344093c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142620"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="c49a0-103">tipo de recurso iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="c49a0-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="c49a0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c49a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c49a0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c49a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c49a0-106">configurações de autenticação Kerberos do iOS para logon único</span><span class="sxs-lookup"><span data-stu-id="c49a0-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="c49a0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c49a0-107">Properties</span></span>
|<span data-ttu-id="c49a0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c49a0-108">Property</span></span>|<span data-ttu-id="c49a0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c49a0-109">Type</span></span>|<span data-ttu-id="c49a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c49a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c49a0-111">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="c49a0-111">allowedAppsList</span></span>|<span data-ttu-id="c49a0-112">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c49a0-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c49a0-113">Lista de identificadores de aplicativos que têm permissão para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="c49a0-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="c49a0-114">Se esse campo for omitido, o logon será aplicado a todos os aplicativos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c49a0-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="c49a0-115">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c49a0-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c49a0-116">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="c49a0-116">allowedUrls</span></span>|<span data-ttu-id="c49a0-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c49a0-117">String collection</span></span>|<span data-ttu-id="c49a0-118">Lista de URLs HTTP que devem ser correspondidas para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="c49a0-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="c49a0-119">Com o iOS 9,0 ou posterior, um caractere curinga pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="c49a0-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="c49a0-120">displayName</span><span class="sxs-lookup"><span data-stu-id="c49a0-120">displayName</span></span>|<span data-ttu-id="c49a0-121">String</span><span class="sxs-lookup"><span data-stu-id="c49a0-121">String</span></span>|<span data-ttu-id="c49a0-122">O nome de exibição das configurações de logon mostradas no dispositivo receptor.</span><span class="sxs-lookup"><span data-stu-id="c49a0-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="c49a0-123">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c49a0-123">kerberosPrincipalName</span></span>|<span data-ttu-id="c49a0-124">String</span><span class="sxs-lookup"><span data-stu-id="c49a0-124">String</span></span>|<span data-ttu-id="c49a0-125">Um nome principal Kerberos.</span><span class="sxs-lookup"><span data-stu-id="c49a0-125">A Kerberos principal name.</span></span> <span data-ttu-id="c49a0-126">Se não for fornecido, o usuário será solicitado a fornecer um durante a instalação do perfil.</span><span class="sxs-lookup"><span data-stu-id="c49a0-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="c49a0-127">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="c49a0-127">kerberosRealm</span></span>|<span data-ttu-id="c49a0-128">String</span><span class="sxs-lookup"><span data-stu-id="c49a0-128">String</span></span>|<span data-ttu-id="c49a0-129">Um nome de realm Kerberos.</span><span class="sxs-lookup"><span data-stu-id="c49a0-129">A Kerberos realm name.</span></span> <span data-ttu-id="c49a0-130">Diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c49a0-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c49a0-131">Relações</span><span class="sxs-lookup"><span data-stu-id="c49a0-131">Relationships</span></span>
<span data-ttu-id="c49a0-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c49a0-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c49a0-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c49a0-133">JSON Representation</span></span>
<span data-ttu-id="c49a0-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c49a0-134">Here is a JSON representation of the resource.</span></span>
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




