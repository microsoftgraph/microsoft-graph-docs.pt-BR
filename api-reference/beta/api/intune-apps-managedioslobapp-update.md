---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5d49e4116dbf6660079e6a2b278b9a2a5890ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168422"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="7e34c-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="7e34c-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="7e34c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e34c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e34c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e34c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e34c-106">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e34c-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e34c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e34c-107">Prerequisites</span></span>
<span data-ttu-id="7e34c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e34c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7e34c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e34c-110">Permission type</span></span>|<span data-ttu-id="7e34c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e34c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e34c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e34c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e34c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e34c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e34c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e34c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e34c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e34c-115">Not supported.</span></span>|
|<span data-ttu-id="7e34c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e34c-116">Application</span></span>|<span data-ttu-id="7e34c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e34c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e34c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e34c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7e34c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e34c-119">Request headers</span></span>
|<span data-ttu-id="7e34c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e34c-120">Header</span></span>|<span data-ttu-id="7e34c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7e34c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e34c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e34c-122">Authorization</span></span>|<span data-ttu-id="7e34c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e34c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e34c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e34c-124">Accept</span></span>|<span data-ttu-id="7e34c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e34c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e34c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e34c-126">Request body</span></span>
<span data-ttu-id="7e34c-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e34c-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="7e34c-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e34c-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="7e34c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e34c-129">Property</span></span>|<span data-ttu-id="7e34c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e34c-130">Type</span></span>|<span data-ttu-id="7e34c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e34c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e34c-132">id</span><span class="sxs-lookup"><span data-stu-id="7e34c-132">id</span></span>|<span data-ttu-id="7e34c-133">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-133">String</span></span>|<span data-ttu-id="7e34c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7e34c-134">Key of the entity.</span></span> <span data-ttu-id="7e34c-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7e34c-136">displayName</span></span>|<span data-ttu-id="7e34c-137">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-137">String</span></span>|<span data-ttu-id="7e34c-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7e34c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7e34c-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-140">description</span><span class="sxs-lookup"><span data-stu-id="7e34c-140">description</span></span>|<span data-ttu-id="7e34c-141">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-141">String</span></span>|<span data-ttu-id="7e34c-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-142">The description of the app.</span></span> <span data-ttu-id="7e34c-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7e34c-144">publisher</span></span>|<span data-ttu-id="7e34c-145">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-145">String</span></span>|<span data-ttu-id="7e34c-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-146">The publisher of the app.</span></span> <span data-ttu-id="7e34c-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7e34c-148">largeIcon</span></span>|[<span data-ttu-id="7e34c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7e34c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7e34c-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7e34c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7e34c-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e34c-152">createdDateTime</span></span>|<span data-ttu-id="7e34c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e34c-153">DateTimeOffset</span></span>|<span data-ttu-id="7e34c-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-154">The date and time the app was created.</span></span> <span data-ttu-id="7e34c-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e34c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7e34c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e34c-157">DateTimeOffset</span></span>|<span data-ttu-id="7e34c-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7e34c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7e34c-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7e34c-160">isFeatured</span></span>|<span data-ttu-id="7e34c-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e34c-161">Boolean</span></span>|<span data-ttu-id="7e34c-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7e34c-163">privacyInformationUrl</span></span>|<span data-ttu-id="7e34c-164">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-164">String</span></span>|<span data-ttu-id="7e34c-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7e34c-165">The privacy statement Url.</span></span> <span data-ttu-id="7e34c-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7e34c-167">informationUrl</span></span>|<span data-ttu-id="7e34c-168">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-168">String</span></span>|<span data-ttu-id="7e34c-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7e34c-169">The more information Url.</span></span> <span data-ttu-id="7e34c-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-171">owner</span><span class="sxs-lookup"><span data-stu-id="7e34c-171">owner</span></span>|<span data-ttu-id="7e34c-172">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-172">String</span></span>|<span data-ttu-id="7e34c-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-173">The owner of the app.</span></span> <span data-ttu-id="7e34c-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-175">developer</span><span class="sxs-lookup"><span data-stu-id="7e34c-175">developer</span></span>|<span data-ttu-id="7e34c-176">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-176">String</span></span>|<span data-ttu-id="7e34c-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-177">The developer of the app.</span></span> <span data-ttu-id="7e34c-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-179">Observações</span><span class="sxs-lookup"><span data-stu-id="7e34c-179">notes</span></span>|<span data-ttu-id="7e34c-180">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-180">String</span></span>|<span data-ttu-id="7e34c-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-181">Notes for the app.</span></span> <span data-ttu-id="7e34c-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7e34c-183">uploadState</span></span>|<span data-ttu-id="7e34c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7e34c-184">Int32</span></span>|<span data-ttu-id="7e34c-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="7e34c-185">The upload state.</span></span> <span data-ttu-id="7e34c-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7e34c-187">publishingState</span></span>|[<span data-ttu-id="7e34c-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7e34c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7e34c-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-189">The publishing state for the app.</span></span> <span data-ttu-id="7e34c-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7e34c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7e34c-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e34c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7e34c-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7e34c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7e34c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7e34c-193">isAssigned</span></span>|<span data-ttu-id="7e34c-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e34c-194">Boolean</span></span>|<span data-ttu-id="7e34c-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7e34c-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e34c-197">roleScopeTagIds</span></span>|<span data-ttu-id="7e34c-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e34c-198">String collection</span></span>|<span data-ttu-id="7e34c-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="7e34c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7e34c-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e34c-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="7e34c-201">appAvailability</span></span>|[<span data-ttu-id="7e34c-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="7e34c-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="7e34c-203">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-203">The Application's availability.</span></span> <span data-ttu-id="7e34c-204">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e34c-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="7e34c-205">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="7e34c-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="7e34c-206">version</span><span class="sxs-lookup"><span data-stu-id="7e34c-206">version</span></span>|<span data-ttu-id="7e34c-207">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-207">String</span></span>|<span data-ttu-id="7e34c-208">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e34c-208">The Application's version.</span></span> <span data-ttu-id="7e34c-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="7e34c-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7e34c-210">committedContentVersion</span></span>|<span data-ttu-id="7e34c-211">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-211">String</span></span>|<span data-ttu-id="7e34c-212">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="7e34c-212">The internal committed content version.</span></span> <span data-ttu-id="7e34c-213">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7e34c-214">fileName</span><span class="sxs-lookup"><span data-stu-id="7e34c-214">fileName</span></span>|<span data-ttu-id="7e34c-215">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-215">String</span></span>|<span data-ttu-id="7e34c-216">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="7e34c-216">The name of the main Lob application file.</span></span> <span data-ttu-id="7e34c-217">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7e34c-218">size</span><span class="sxs-lookup"><span data-stu-id="7e34c-218">size</span></span>|<span data-ttu-id="7e34c-219">Int64</span><span class="sxs-lookup"><span data-stu-id="7e34c-219">Int64</span></span>|<span data-ttu-id="7e34c-220">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="7e34c-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="7e34c-221">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e34c-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7e34c-222">bundleId</span><span class="sxs-lookup"><span data-stu-id="7e34c-222">bundleId</span></span>|<span data-ttu-id="7e34c-223">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-223">String</span></span>|<span data-ttu-id="7e34c-224">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7e34c-224">The Identity Name.</span></span>|
|<span data-ttu-id="7e34c-225">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="7e34c-225">applicableDeviceType</span></span>|[<span data-ttu-id="7e34c-226">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="7e34c-226">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="7e34c-227">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="7e34c-227">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="7e34c-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7e34c-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7e34c-229">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7e34c-229">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="7e34c-230">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="7e34c-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7e34c-231">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7e34c-231">expirationDateTime</span></span>|<span data-ttu-id="7e34c-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e34c-232">DateTimeOffset</span></span>|<span data-ttu-id="7e34c-233">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="7e34c-233">The expiration time.</span></span>|
|<span data-ttu-id="7e34c-234">versionNumber</span><span class="sxs-lookup"><span data-stu-id="7e34c-234">versionNumber</span></span>|<span data-ttu-id="7e34c-235">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-235">String</span></span>|<span data-ttu-id="7e34c-236">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7e34c-236">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7e34c-237">buildNumber</span><span class="sxs-lookup"><span data-stu-id="7e34c-237">buildNumber</span></span>|<span data-ttu-id="7e34c-238">String</span><span class="sxs-lookup"><span data-stu-id="7e34c-238">String</span></span>|<span data-ttu-id="7e34c-239">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7e34c-239">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7e34c-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7e34c-240">identityVersion</span></span>|<span data-ttu-id="7e34c-241">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e34c-241">String</span></span>|<span data-ttu-id="7e34c-242">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="7e34c-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="7e34c-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e34c-243">Response</span></span>
<span data-ttu-id="7e34c-244">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e34c-244">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e34c-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e34c-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e34c-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e34c-246">Request</span></span>
<span data-ttu-id="7e34c-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e34c-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1442

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="7e34c-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e34c-248">Response</span></span>
<span data-ttu-id="7e34c-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e34c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1614

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




