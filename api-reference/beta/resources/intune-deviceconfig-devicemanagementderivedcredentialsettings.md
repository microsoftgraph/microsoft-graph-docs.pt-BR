---
title: tipo de recurso deviceManagementDerivedCredentialSettings
description: Entidade que descreve as configurações de nível de locatário para credenciais derivadas
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 06f87b7c2f94bcd95d27889bfb9ee0649c4aae92
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990019"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="25619-103">tipo de recurso deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="25619-103">deviceManagementDerivedCredentialSettings resource type</span></span>

> <span data-ttu-id="25619-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25619-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25619-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25619-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25619-106">Entidade que descreve as configurações de nível de locatário para credenciais derivadas</span><span class="sxs-lookup"><span data-stu-id="25619-106">Entity that describes tenant level settings for derived credentials</span></span>

## <a name="methods"></a><span data-ttu-id="25619-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="25619-107">Methods</span></span>
|<span data-ttu-id="25619-108">Método</span><span class="sxs-lookup"><span data-stu-id="25619-108">Method</span></span>|<span data-ttu-id="25619-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="25619-109">Return Type</span></span>|<span data-ttu-id="25619-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="25619-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="25619-111">Obter deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="25619-111">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="25619-112">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="25619-112">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="25619-113">Leia as propriedades e as relações do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="25619-113">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="25619-114">Atualizar deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="25619-114">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="25619-115">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="25619-115">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="25619-116">Atualiza as propriedades de um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="25619-116">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="25619-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25619-117">Properties</span></span>
|<span data-ttu-id="25619-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25619-118">Property</span></span>|<span data-ttu-id="25619-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="25619-119">Type</span></span>|<span data-ttu-id="25619-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="25619-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25619-121">id</span><span class="sxs-lookup"><span data-stu-id="25619-121">id</span></span>|<span data-ttu-id="25619-122">String</span><span class="sxs-lookup"><span data-stu-id="25619-122">String</span></span>|<span data-ttu-id="25619-123">Identificador exclusivo para a credencial derivada</span><span class="sxs-lookup"><span data-stu-id="25619-123">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="25619-124">helpUrl</span><span class="sxs-lookup"><span data-stu-id="25619-124">helpUrl</span></span>|<span data-ttu-id="25619-125">String</span><span class="sxs-lookup"><span data-stu-id="25619-125">String</span></span>|<span data-ttu-id="25619-126">A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="25619-126">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="25619-127">displayName</span><span class="sxs-lookup"><span data-stu-id="25619-127">displayName</span></span>|<span data-ttu-id="25619-128">String</span><span class="sxs-lookup"><span data-stu-id="25619-128">String</span></span>|<span data-ttu-id="25619-129">O nome de exibição do perfil.</span><span class="sxs-lookup"><span data-stu-id="25619-129">The display name for the profile.</span></span>|
|<span data-ttu-id="25619-130">emissor</span><span class="sxs-lookup"><span data-stu-id="25619-130">issuer</span></span>|[<span data-ttu-id="25619-131">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="25619-131">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="25619-132">O provedor de credenciais derivado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="25619-132">The derived credential provider to use.</span></span> <span data-ttu-id="25619-133">Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="25619-133">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="25619-134">notificationType</span><span class="sxs-lookup"><span data-stu-id="25619-134">notificationType</span></span>|[<span data-ttu-id="25619-135">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="25619-135">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="25619-136">Os métodos usados para informar ao usuário final para abrir o portal da empresa para entregar os perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25619-136">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="25619-137">Os valores possíveis são: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="25619-137">Possible values are: `none`, `companyPortal`, `email`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25619-138">Relações</span><span class="sxs-lookup"><span data-stu-id="25619-138">Relationships</span></span>
<span data-ttu-id="25619-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25619-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25619-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25619-140">JSON Representation</span></span>
<span data-ttu-id="25619-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25619-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```





