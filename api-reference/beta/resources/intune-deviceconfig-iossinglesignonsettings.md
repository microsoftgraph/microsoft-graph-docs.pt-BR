---
title: tipo de recurso iosSingleSignOnSettings
description: configurações de autenticação Kerberos do iOS para logon único
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11875bb07b87cf8c9415660f5961dafa73f54f57
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995613"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="ae047-103">tipo de recurso iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="ae047-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="ae047-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae047-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae047-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae047-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae047-106">configurações de autenticação Kerberos do iOS para logon único</span><span class="sxs-lookup"><span data-stu-id="ae047-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="ae047-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae047-107">Properties</span></span>
|<span data-ttu-id="ae047-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae047-108">Property</span></span>|<span data-ttu-id="ae047-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae047-109">Type</span></span>|<span data-ttu-id="ae047-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae047-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae047-111">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="ae047-111">allowedAppsList</span></span>|<span data-ttu-id="ae047-112">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ae047-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ae047-113">Lista de identificadores de aplicativos que têm permissão para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="ae047-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="ae047-114">Se esse campo for omitido, o logon será aplicado a todos os aplicativos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ae047-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="ae047-115">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ae047-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ae047-116">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="ae047-116">allowedUrls</span></span>|<span data-ttu-id="ae047-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae047-117">String collection</span></span>|<span data-ttu-id="ae047-118">Lista de URLs HTTP que devem ser correspondidas para usar esse logon.</span><span class="sxs-lookup"><span data-stu-id="ae047-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="ae047-119">Com o iOS 9,0 ou posterior, um caractere curinga pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="ae047-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="ae047-120">displayName</span><span class="sxs-lookup"><span data-stu-id="ae047-120">displayName</span></span>|<span data-ttu-id="ae047-121">String</span><span class="sxs-lookup"><span data-stu-id="ae047-121">String</span></span>|<span data-ttu-id="ae047-122">O nome de exibição das configurações de logon mostradas no dispositivo receptor.</span><span class="sxs-lookup"><span data-stu-id="ae047-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="ae047-123">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae047-123">kerberosPrincipalName</span></span>|<span data-ttu-id="ae047-124">String</span><span class="sxs-lookup"><span data-stu-id="ae047-124">String</span></span>|<span data-ttu-id="ae047-125">Um nome principal Kerberos.</span><span class="sxs-lookup"><span data-stu-id="ae047-125">A Kerberos principal name.</span></span> <span data-ttu-id="ae047-126">Se não for fornecido, o usuário será solicitado a fornecer um durante a instalação do perfil.</span><span class="sxs-lookup"><span data-stu-id="ae047-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="ae047-127">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="ae047-127">kerberosRealm</span></span>|<span data-ttu-id="ae047-128">String</span><span class="sxs-lookup"><span data-stu-id="ae047-128">String</span></span>|<span data-ttu-id="ae047-129">Um nome de realm Kerberos.</span><span class="sxs-lookup"><span data-stu-id="ae047-129">A Kerberos realm name.</span></span> <span data-ttu-id="ae047-130">Diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ae047-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae047-131">Relações</span><span class="sxs-lookup"><span data-stu-id="ae047-131">Relationships</span></span>
<span data-ttu-id="ae047-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae047-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae047-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae047-133">JSON Representation</span></span>
<span data-ttu-id="ae047-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae047-134">Here is a JSON representation of the resource.</span></span>
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





