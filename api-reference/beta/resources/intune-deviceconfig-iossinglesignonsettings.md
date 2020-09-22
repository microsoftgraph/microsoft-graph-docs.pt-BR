---
title: tipo de recurso iosSingleSignOnSettings
description: configurações de autenticação Kerberos do iOS para logon único
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6206dbc62fa8ae9ff0dee4d47bec30ce4ae99ae0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003637"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="393d5-103">tipo de recurso iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="393d5-103">iosSingleSignOnSettings resource type</span></span>

<span data-ttu-id="393d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="393d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="393d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="393d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="393d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="393d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="393d5-107">configurações de autenticação Kerberos do iOS para logon único</span><span class="sxs-lookup"><span data-stu-id="393d5-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="393d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="393d5-108">Properties</span></span>
|<span data-ttu-id="393d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="393d5-109">Property</span></span>|<span data-ttu-id="393d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="393d5-110">Type</span></span>|<span data-ttu-id="393d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="393d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393d5-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="393d5-112">allowedAppsList</span></span>|<span data-ttu-id="393d5-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="393d5-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="393d5-114">Lista de identificadores de aplicativos que têm permissão para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="393d5-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="393d5-115">Se esse campo for omitido, o logon será aplicado a todos os aplicativos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="393d5-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="393d5-116">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="393d5-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="393d5-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="393d5-117">allowedUrls</span></span>|<span data-ttu-id="393d5-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="393d5-118">String collection</span></span>|<span data-ttu-id="393d5-119">Lista de URLs HTTP que devem ser correspondidas para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="393d5-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="393d5-120">Com o iOS 9,0 ou posterior, um caractere curinga pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="393d5-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="393d5-121">displayName</span><span class="sxs-lookup"><span data-stu-id="393d5-121">displayName</span></span>|<span data-ttu-id="393d5-122">String</span><span class="sxs-lookup"><span data-stu-id="393d5-122">String</span></span>|<span data-ttu-id="393d5-123">O nome de exibição das configurações de logon mostradas no dispositivo receptor.</span><span class="sxs-lookup"><span data-stu-id="393d5-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="393d5-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="393d5-124">kerberosPrincipalName</span></span>|<span data-ttu-id="393d5-125">String</span><span class="sxs-lookup"><span data-stu-id="393d5-125">String</span></span>|<span data-ttu-id="393d5-126">Um nome principal Kerberos.</span><span class="sxs-lookup"><span data-stu-id="393d5-126">A Kerberos principal name.</span></span> <span data-ttu-id="393d5-127">Se não for fornecido, o usuário será solicitado a fornecer um durante a instalação do perfil.</span><span class="sxs-lookup"><span data-stu-id="393d5-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="393d5-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="393d5-128">kerberosRealm</span></span>|<span data-ttu-id="393d5-129">String</span><span class="sxs-lookup"><span data-stu-id="393d5-129">String</span></span>|<span data-ttu-id="393d5-130">Um nome de realm Kerberos.</span><span class="sxs-lookup"><span data-stu-id="393d5-130">A Kerberos realm name.</span></span> <span data-ttu-id="393d5-131">Diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="393d5-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="393d5-132">Relações</span><span class="sxs-lookup"><span data-stu-id="393d5-132">Relationships</span></span>
<span data-ttu-id="393d5-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="393d5-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="393d5-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="393d5-134">JSON Representation</span></span>
<span data-ttu-id="393d5-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="393d5-135">Here is a JSON representation of the resource.</span></span>
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






