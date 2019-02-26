---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6029450f517e08876c124b9f5bcfb7e0b6d31880
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151909"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="698e2-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="698e2-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="698e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="698e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="698e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="698e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="698e2-106">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="698e2-106">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="698e2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="698e2-107">Prerequisites</span></span>
<span data-ttu-id="698e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="698e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="698e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="698e2-110">Permission type</span></span>|<span data-ttu-id="698e2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="698e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="698e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="698e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="698e2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698e2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="698e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="698e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="698e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="698e2-115">Not supported.</span></span>|
|<span data-ttu-id="698e2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="698e2-116">Application</span></span>|<span data-ttu-id="698e2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="698e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="698e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="698e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="698e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="698e2-119">Request headers</span></span>
|<span data-ttu-id="698e2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="698e2-120">Header</span></span>|<span data-ttu-id="698e2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="698e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="698e2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="698e2-122">Authorization</span></span>|<span data-ttu-id="698e2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="698e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="698e2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="698e2-124">Accept</span></span>|<span data-ttu-id="698e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="698e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="698e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="698e2-126">Request body</span></span>
<span data-ttu-id="698e2-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="698e2-127">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="698e2-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="698e2-128">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="698e2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="698e2-129">Property</span></span>|<span data-ttu-id="698e2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="698e2-130">Type</span></span>|<span data-ttu-id="698e2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="698e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="698e2-132">id</span><span class="sxs-lookup"><span data-stu-id="698e2-132">id</span></span>|<span data-ttu-id="698e2-133">String</span><span class="sxs-lookup"><span data-stu-id="698e2-133">String</span></span>|<span data-ttu-id="698e2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="698e2-134">Key of the entity.</span></span> <span data-ttu-id="698e2-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="698e2-136">displayName</span></span>|<span data-ttu-id="698e2-137">String</span><span class="sxs-lookup"><span data-stu-id="698e2-137">String</span></span>|<span data-ttu-id="698e2-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="698e2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="698e2-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-140">description</span><span class="sxs-lookup"><span data-stu-id="698e2-140">description</span></span>|<span data-ttu-id="698e2-141">String</span><span class="sxs-lookup"><span data-stu-id="698e2-141">String</span></span>|<span data-ttu-id="698e2-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-142">The description of the app.</span></span> <span data-ttu-id="698e2-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="698e2-144">publisher</span></span>|<span data-ttu-id="698e2-145">String</span><span class="sxs-lookup"><span data-stu-id="698e2-145">String</span></span>|<span data-ttu-id="698e2-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-146">The publisher of the app.</span></span> <span data-ttu-id="698e2-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="698e2-148">largeIcon</span></span>|[<span data-ttu-id="698e2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="698e2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="698e2-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="698e2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="698e2-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="698e2-152">createdDateTime</span></span>|<span data-ttu-id="698e2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="698e2-153">DateTimeOffset</span></span>|<span data-ttu-id="698e2-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-154">The date and time the app was created.</span></span> <span data-ttu-id="698e2-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="698e2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="698e2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="698e2-157">DateTimeOffset</span></span>|<span data-ttu-id="698e2-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="698e2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="698e2-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="698e2-160">isFeatured</span></span>|<span data-ttu-id="698e2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="698e2-161">Boolean</span></span>|<span data-ttu-id="698e2-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="698e2-163">privacyInformationUrl</span></span>|<span data-ttu-id="698e2-164">String</span><span class="sxs-lookup"><span data-stu-id="698e2-164">String</span></span>|<span data-ttu-id="698e2-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="698e2-165">The privacy statement Url.</span></span> <span data-ttu-id="698e2-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="698e2-167">informationUrl</span></span>|<span data-ttu-id="698e2-168">String</span><span class="sxs-lookup"><span data-stu-id="698e2-168">String</span></span>|<span data-ttu-id="698e2-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="698e2-169">The more information Url.</span></span> <span data-ttu-id="698e2-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-171">owner</span><span class="sxs-lookup"><span data-stu-id="698e2-171">owner</span></span>|<span data-ttu-id="698e2-172">String</span><span class="sxs-lookup"><span data-stu-id="698e2-172">String</span></span>|<span data-ttu-id="698e2-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="698e2-173">The owner of the app.</span></span> <span data-ttu-id="698e2-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-175">developer</span><span class="sxs-lookup"><span data-stu-id="698e2-175">developer</span></span>|<span data-ttu-id="698e2-176">String</span><span class="sxs-lookup"><span data-stu-id="698e2-176">String</span></span>|<span data-ttu-id="698e2-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-177">The developer of the app.</span></span> <span data-ttu-id="698e2-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-179">Observações</span><span class="sxs-lookup"><span data-stu-id="698e2-179">notes</span></span>|<span data-ttu-id="698e2-180">String</span><span class="sxs-lookup"><span data-stu-id="698e2-180">String</span></span>|<span data-ttu-id="698e2-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-181">Notes for the app.</span></span> <span data-ttu-id="698e2-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="698e2-183">uploadState</span></span>|<span data-ttu-id="698e2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="698e2-184">Int32</span></span>|<span data-ttu-id="698e2-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="698e2-185">The upload state.</span></span> <span data-ttu-id="698e2-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="698e2-187">publishingState</span></span>|[<span data-ttu-id="698e2-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="698e2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="698e2-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-189">The publishing state for the app.</span></span> <span data-ttu-id="698e2-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="698e2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="698e2-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="698e2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="698e2-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="698e2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="698e2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="698e2-193">isAssigned</span></span>|<span data-ttu-id="698e2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="698e2-194">Boolean</span></span>|<span data-ttu-id="698e2-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="698e2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="698e2-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="698e2-197">roleScopeTagIds</span></span>|<span data-ttu-id="698e2-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="698e2-198">String collection</span></span>|<span data-ttu-id="698e2-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="698e2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="698e2-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="698e2-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="698e2-201">appAvailability</span></span>|[<span data-ttu-id="698e2-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="698e2-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="698e2-203">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-203">The Application's availability.</span></span> <span data-ttu-id="698e2-204">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="698e2-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="698e2-205">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="698e2-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="698e2-206">version</span><span class="sxs-lookup"><span data-stu-id="698e2-206">version</span></span>|<span data-ttu-id="698e2-207">String</span><span class="sxs-lookup"><span data-stu-id="698e2-207">String</span></span>|<span data-ttu-id="698e2-208">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="698e2-208">The Application's version.</span></span> <span data-ttu-id="698e2-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="698e2-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="698e2-210">committedContentVersion</span></span>|<span data-ttu-id="698e2-211">String</span><span class="sxs-lookup"><span data-stu-id="698e2-211">String</span></span>|<span data-ttu-id="698e2-212">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="698e2-212">The internal committed content version.</span></span> <span data-ttu-id="698e2-213">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="698e2-214">fileName</span><span class="sxs-lookup"><span data-stu-id="698e2-214">fileName</span></span>|<span data-ttu-id="698e2-215">String</span><span class="sxs-lookup"><span data-stu-id="698e2-215">String</span></span>|<span data-ttu-id="698e2-216">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="698e2-216">The name of the main Lob application file.</span></span> <span data-ttu-id="698e2-217">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="698e2-218">size</span><span class="sxs-lookup"><span data-stu-id="698e2-218">size</span></span>|<span data-ttu-id="698e2-219">Int64</span><span class="sxs-lookup"><span data-stu-id="698e2-219">Int64</span></span>|<span data-ttu-id="698e2-220">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="698e2-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="698e2-221">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="698e2-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="698e2-222">packageId</span><span class="sxs-lookup"><span data-stu-id="698e2-222">packageId</span></span>|<span data-ttu-id="698e2-223">String</span><span class="sxs-lookup"><span data-stu-id="698e2-223">String</span></span>|<span data-ttu-id="698e2-224">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="698e2-224">The package identifier.</span></span>|
|<span data-ttu-id="698e2-225">identityName</span><span class="sxs-lookup"><span data-stu-id="698e2-225">identityName</span></span>|<span data-ttu-id="698e2-226">String</span><span class="sxs-lookup"><span data-stu-id="698e2-226">String</span></span>|<span data-ttu-id="698e2-227">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="698e2-227">The Identity Name.</span></span>|
|<span data-ttu-id="698e2-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="698e2-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="698e2-229">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="698e2-229">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="698e2-230">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="698e2-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="698e2-231">versionName</span><span class="sxs-lookup"><span data-stu-id="698e2-231">versionName</span></span>|<span data-ttu-id="698e2-232">String</span><span class="sxs-lookup"><span data-stu-id="698e2-232">String</span></span>|<span data-ttu-id="698e2-233">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="698e2-233">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="698e2-234">versionCode</span><span class="sxs-lookup"><span data-stu-id="698e2-234">versionCode</span></span>|<span data-ttu-id="698e2-235">String</span><span class="sxs-lookup"><span data-stu-id="698e2-235">String</span></span>|<span data-ttu-id="698e2-236">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="698e2-236">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="698e2-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="698e2-237">identityVersion</span></span>|<span data-ttu-id="698e2-238">String</span><span class="sxs-lookup"><span data-stu-id="698e2-238">String</span></span>|<span data-ttu-id="698e2-239">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="698e2-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="698e2-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="698e2-240">Response</span></span>
<span data-ttu-id="698e2-241">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="698e2-241">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="698e2-242">Exemplo</span><span class="sxs-lookup"><span data-stu-id="698e2-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="698e2-243">Solicitação</span><span class="sxs-lookup"><span data-stu-id="698e2-243">Request</span></span>
<span data-ttu-id="698e2-244">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="698e2-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1464

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="698e2-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="698e2-245">Response</span></span>
<span data-ttu-id="698e2-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="698e2-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1636

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




