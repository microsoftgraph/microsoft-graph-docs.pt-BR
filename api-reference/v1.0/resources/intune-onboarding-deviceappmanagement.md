---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae8bd6389d40b45d59d82d183fcfa6b3a2327367
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752945"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="1fda1-103">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1fda1-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="1fda1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fda1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fda1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fda1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fda1-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1fda1-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="1fda1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1fda1-107">Methods</span></span>
|<span data-ttu-id="1fda1-108">Método</span><span class="sxs-lookup"><span data-stu-id="1fda1-108">Method</span></span>|<span data-ttu-id="1fda1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1fda1-109">Return Type</span></span>|<span data-ttu-id="1fda1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fda1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1fda1-111">Obter deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1fda1-111">Get deviceAppManagement</span></span>](../api/intune-onboarding-deviceappmanagement-get.md)|[<span data-ttu-id="1fda1-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1fda1-112">deviceAppManagement</span></span>](../resources/intune-onboarding-deviceappmanagement.md)|<span data-ttu-id="1fda1-113">Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1fda1-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="1fda1-114">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1fda1-114">Update deviceAppManagement</span></span>](../api/intune-onboarding-deviceappmanagement-update.md)|[<span data-ttu-id="1fda1-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1fda1-115">deviceAppManagement</span></span>](../resources/intune-onboarding-deviceappmanagement.md)|<span data-ttu-id="1fda1-116">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1fda1-116">Update the properties of a [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="1fda1-117">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="1fda1-117">syncMicrosoftStoreForBusinessApps action</span></span>](../api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|<span data-ttu-id="1fda1-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fda1-118">None</span></span>|<span data-ttu-id="1fda1-119">Sincroniza a conta do Intune com o Microsoft Store para Empresas</span><span class="sxs-lookup"><span data-stu-id="1fda1-119">Syncs Intune account with Microsoft Store For Business</span></span>|

## <a name="properties"></a><span data-ttu-id="1fda1-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fda1-120">Properties</span></span>
|<span data-ttu-id="1fda1-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fda1-121">Property</span></span>|<span data-ttu-id="1fda1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fda1-122">Type</span></span>|<span data-ttu-id="1fda1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fda1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fda1-124">id</span><span class="sxs-lookup"><span data-stu-id="1fda1-124">id</span></span>|<span data-ttu-id="1fda1-125">String</span><span class="sxs-lookup"><span data-stu-id="1fda1-125">String</span></span>|<span data-ttu-id="1fda1-126">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1fda1-126">Not yet documented</span></span>|
|<span data-ttu-id="1fda1-127">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1fda1-127">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1fda1-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fda1-128">DateTimeOffset</span></span>|<span data-ttu-id="1fda1-129">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="1fda1-129">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="1fda1-130">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="1fda1-130">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="1fda1-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fda1-131">Boolean</span></span>|<span data-ttu-id="1fda1-132">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="1fda1-132">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="1fda1-133">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="1fda1-133">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="1fda1-134">String</span><span class="sxs-lookup"><span data-stu-id="1fda1-134">String</span></span>|<span data-ttu-id="1fda1-135">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="1fda1-135">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="1fda1-136">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="1fda1-136">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="1fda1-137">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="1fda1-137">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="1fda1-138">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="1fda1-138">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="1fda1-139">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="1fda1-139">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="1fda1-140">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="1fda1-140">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="1fda1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fda1-141">DateTimeOffset</span></span>|<span data-ttu-id="1fda1-142">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="1fda1-142">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fda1-143">Relações</span><span class="sxs-lookup"><span data-stu-id="1fda1-143">Relationships</span></span>
|<span data-ttu-id="1fda1-144">Relação</span><span class="sxs-lookup"><span data-stu-id="1fda1-144">Relationship</span></span>|<span data-ttu-id="1fda1-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fda1-145">Type</span></span>|<span data-ttu-id="1fda1-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fda1-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fda1-147">vppTokens</span><span class="sxs-lookup"><span data-stu-id="1fda1-147">vppTokens</span></span>|<span data-ttu-id="1fda1-148">Coleção de [vppToken](../resources/intune-onboarding-vpptoken.md)</span><span class="sxs-lookup"><span data-stu-id="1fda1-148">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="1fda1-149">Lista de tokens Vpp desta organização.</span><span class="sxs-lookup"><span data-stu-id="1fda1-149">List of Vpp tokens for this organization.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fda1-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fda1-150">JSON Representation</span></span>
<span data-ttu-id="1fda1-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fda1-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```




