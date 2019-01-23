---
title: tipo de recurso de iosSingleSignOnSettings
description: iOS configurações de autenticação Kerberos de single sign-on
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421316"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="a7e90-103">tipo de recurso de iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a7e90-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="a7e90-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7e90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7e90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7e90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7e90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a7e90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7e90-107">iOS configurações de autenticação Kerberos de single sign-on</span><span class="sxs-lookup"><span data-stu-id="a7e90-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="a7e90-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7e90-108">Properties</span></span>
|<span data-ttu-id="a7e90-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7e90-109">Property</span></span>|<span data-ttu-id="a7e90-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7e90-110">Type</span></span>|<span data-ttu-id="a7e90-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7e90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e90-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="a7e90-112">allowedAppsList</span></span>|<span data-ttu-id="a7e90-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a7e90-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a7e90-114">Lista de identificadores de aplicativo que têm permissão para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="a7e90-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="a7e90-115">Se esse campo for omitido, o login se aplica a todos os aplicativos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7e90-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="a7e90-116">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a7e90-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a7e90-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="a7e90-117">allowedUrls</span></span>|<span data-ttu-id="a7e90-118">String collection</span><span class="sxs-lookup"><span data-stu-id="a7e90-118">String collection</span></span>|<span data-ttu-id="a7e90-119">Lista das URLs de HTTP que deve coincidir para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="a7e90-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="a7e90-120">Com o iOS 9.0 ou posterior, um caracteres curinga podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="a7e90-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="a7e90-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a7e90-121">displayName</span></span>|<span data-ttu-id="a7e90-122">String</span><span class="sxs-lookup"><span data-stu-id="a7e90-122">String</span></span>|<span data-ttu-id="a7e90-123">O nome de exibição das configurações de logon mostrado no dispositivo receptor.</span><span class="sxs-lookup"><span data-stu-id="a7e90-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="a7e90-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7e90-124">kerberosPrincipalName</span></span>|<span data-ttu-id="a7e90-125">String</span><span class="sxs-lookup"><span data-stu-id="a7e90-125">String</span></span>|<span data-ttu-id="a7e90-126">Um nome UPN do Kerberos.</span><span class="sxs-lookup"><span data-stu-id="a7e90-126">A Kerberos principal name.</span></span> <span data-ttu-id="a7e90-127">Se não fornecido, o usuário é solicitado por um durante a instalação do perfil.</span><span class="sxs-lookup"><span data-stu-id="a7e90-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="a7e90-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="a7e90-128">kerberosRealm</span></span>|<span data-ttu-id="a7e90-129">String</span><span class="sxs-lookup"><span data-stu-id="a7e90-129">String</span></span>|<span data-ttu-id="a7e90-130">Um nome de realm Kerberos.</span><span class="sxs-lookup"><span data-stu-id="a7e90-130">A Kerberos realm name.</span></span> <span data-ttu-id="a7e90-131">Maiusculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a7e90-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7e90-132">Relações</span><span class="sxs-lookup"><span data-stu-id="a7e90-132">Relationships</span></span>
<span data-ttu-id="a7e90-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7e90-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7e90-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7e90-134">JSON Representation</span></span>
<span data-ttu-id="a7e90-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7e90-135">Here is a JSON representation of the resource.</span></span>
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




