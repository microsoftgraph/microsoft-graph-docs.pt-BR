---
title: tipo de recurso de iosSingleSignOnSettings
description: iOS configurações de autenticação Kerberos de single sign-on
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54c5656de6262692324cce8ab71a0e100672c050
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952668"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="a0f78-103">tipo de recurso de iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a0f78-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="a0f78-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0f78-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0f78-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0f78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0f78-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0f78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0f78-107">iOS configurações de autenticação Kerberos de single sign-on</span><span class="sxs-lookup"><span data-stu-id="a0f78-107">iOS Kerberos authentication settings for single sign-on</span></span>
## <a name="properties"></a><span data-ttu-id="a0f78-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0f78-108">Properties</span></span>
|<span data-ttu-id="a0f78-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0f78-109">Property</span></span>|<span data-ttu-id="a0f78-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0f78-110">Type</span></span>|<span data-ttu-id="a0f78-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0f78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0f78-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="a0f78-112">allowedAppsList</span></span>|<span data-ttu-id="a0f78-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a0f78-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a0f78-114">Lista de identificadores de aplicativo que têm permissão para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="a0f78-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="a0f78-115">Se esse campo for omitido, o login se aplica a todos os aplicativos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0f78-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="a0f78-116">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a0f78-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a0f78-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="a0f78-117">allowedUrls</span></span>|<span data-ttu-id="a0f78-118">String collection</span><span class="sxs-lookup"><span data-stu-id="a0f78-118">String collection</span></span>|<span data-ttu-id="a0f78-119">Lista das URLs de HTTP que deve coincidir para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="a0f78-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="a0f78-120">Com o iOS 9.0 ou posterior, um caracteres curinga podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="a0f78-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="a0f78-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a0f78-121">displayName</span></span>|<span data-ttu-id="a0f78-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0f78-122">String</span></span>|<span data-ttu-id="a0f78-123">O nome de exibição das configurações de logon mostrado no dispositivo receptor.</span><span class="sxs-lookup"><span data-stu-id="a0f78-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="a0f78-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a0f78-124">kerberosPrincipalName</span></span>|<span data-ttu-id="a0f78-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0f78-125">String</span></span>|<span data-ttu-id="a0f78-126">Um nome UPN do Kerberos.</span><span class="sxs-lookup"><span data-stu-id="a0f78-126">A Kerberos principal name.</span></span> <span data-ttu-id="a0f78-127">Se não fornecido, o usuário é solicitado por um durante a instalação do perfil.</span><span class="sxs-lookup"><span data-stu-id="a0f78-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="a0f78-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="a0f78-128">kerberosRealm</span></span>|<span data-ttu-id="a0f78-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0f78-129">String</span></span>|<span data-ttu-id="a0f78-130">Um nome de realm Kerberos.</span><span class="sxs-lookup"><span data-stu-id="a0f78-130">A Kerberos realm name.</span></span> <span data-ttu-id="a0f78-131">Maiusculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a0f78-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0f78-132">Relações</span><span class="sxs-lookup"><span data-stu-id="a0f78-132">Relationships</span></span>
<span data-ttu-id="a0f78-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0f78-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0f78-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0f78-134">JSON Representation</span></span>
<span data-ttu-id="a0f78-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0f78-135">Here is a JSON representation of the resource.</span></span>
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





