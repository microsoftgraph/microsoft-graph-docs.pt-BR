---
title: Atualizar androidLobApp
description: Atualiza as propriedades de um objeto androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 101374a08b2ed6c74ad528d5ac5391b23ce64d54
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175406"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="f8007-103">Atualizar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="f8007-103">Update androidLobApp</span></span>

> <span data-ttu-id="f8007-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8007-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8007-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8007-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8007-106">Atualiza as propriedades de um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8007-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8007-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8007-107">Prerequisites</span></span>
<span data-ttu-id="f8007-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f8007-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8007-110">Permission type</span></span>|<span data-ttu-id="f8007-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8007-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8007-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8007-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8007-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8007-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8007-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8007-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8007-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8007-115">Not supported.</span></span>|
|<span data-ttu-id="f8007-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8007-116">Application</span></span>|<span data-ttu-id="f8007-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8007-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8007-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8007-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f8007-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8007-119">Request headers</span></span>
|<span data-ttu-id="f8007-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8007-120">Header</span></span>|<span data-ttu-id="f8007-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8007-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8007-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8007-122">Authorization</span></span>|<span data-ttu-id="f8007-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8007-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8007-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8007-124">Accept</span></span>|<span data-ttu-id="f8007-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8007-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8007-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8007-126">Request body</span></span>
<span data-ttu-id="f8007-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8007-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="f8007-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8007-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="f8007-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8007-129">Property</span></span>|<span data-ttu-id="f8007-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8007-130">Type</span></span>|<span data-ttu-id="f8007-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8007-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8007-132">id</span><span class="sxs-lookup"><span data-stu-id="f8007-132">id</span></span>|<span data-ttu-id="f8007-133">String</span><span class="sxs-lookup"><span data-stu-id="f8007-133">String</span></span>|<span data-ttu-id="f8007-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8007-134">Key of the entity.</span></span> <span data-ttu-id="f8007-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f8007-136">displayName</span></span>|<span data-ttu-id="f8007-137">String</span><span class="sxs-lookup"><span data-stu-id="f8007-137">String</span></span>|<span data-ttu-id="f8007-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f8007-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f8007-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-140">description</span><span class="sxs-lookup"><span data-stu-id="f8007-140">description</span></span>|<span data-ttu-id="f8007-141">String</span><span class="sxs-lookup"><span data-stu-id="f8007-141">String</span></span>|<span data-ttu-id="f8007-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8007-142">The description of the app.</span></span> <span data-ttu-id="f8007-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f8007-144">publisher</span></span>|<span data-ttu-id="f8007-145">String</span><span class="sxs-lookup"><span data-stu-id="f8007-145">String</span></span>|<span data-ttu-id="f8007-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8007-146">The publisher of the app.</span></span> <span data-ttu-id="f8007-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f8007-148">largeIcon</span></span>|[<span data-ttu-id="f8007-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f8007-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f8007-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f8007-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f8007-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8007-152">createdDateTime</span></span>|<span data-ttu-id="f8007-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8007-153">DateTimeOffset</span></span>|<span data-ttu-id="f8007-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8007-154">The date and time the app was created.</span></span> <span data-ttu-id="f8007-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8007-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f8007-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8007-157">DateTimeOffset</span></span>|<span data-ttu-id="f8007-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f8007-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f8007-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f8007-160">isFeatured</span></span>|<span data-ttu-id="f8007-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8007-161">Boolean</span></span>|<span data-ttu-id="f8007-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f8007-163">privacyInformationUrl</span></span>|<span data-ttu-id="f8007-164">String</span><span class="sxs-lookup"><span data-stu-id="f8007-164">String</span></span>|<span data-ttu-id="f8007-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f8007-165">The privacy statement Url.</span></span> <span data-ttu-id="f8007-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f8007-167">informationUrl</span></span>|<span data-ttu-id="f8007-168">String</span><span class="sxs-lookup"><span data-stu-id="f8007-168">String</span></span>|<span data-ttu-id="f8007-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f8007-169">The more information Url.</span></span> <span data-ttu-id="f8007-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-171">owner</span><span class="sxs-lookup"><span data-stu-id="f8007-171">owner</span></span>|<span data-ttu-id="f8007-172">String</span><span class="sxs-lookup"><span data-stu-id="f8007-172">String</span></span>|<span data-ttu-id="f8007-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f8007-173">The owner of the app.</span></span> <span data-ttu-id="f8007-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-175">developer</span><span class="sxs-lookup"><span data-stu-id="f8007-175">developer</span></span>|<span data-ttu-id="f8007-176">String</span><span class="sxs-lookup"><span data-stu-id="f8007-176">String</span></span>|<span data-ttu-id="f8007-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8007-177">The developer of the app.</span></span> <span data-ttu-id="f8007-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-179">Observações</span><span class="sxs-lookup"><span data-stu-id="f8007-179">notes</span></span>|<span data-ttu-id="f8007-180">String</span><span class="sxs-lookup"><span data-stu-id="f8007-180">String</span></span>|<span data-ttu-id="f8007-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8007-181">Notes for the app.</span></span> <span data-ttu-id="f8007-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f8007-183">uploadState</span></span>|<span data-ttu-id="f8007-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f8007-184">Int32</span></span>|<span data-ttu-id="f8007-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="f8007-185">The upload state.</span></span> <span data-ttu-id="f8007-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f8007-187">publishingState</span></span>|[<span data-ttu-id="f8007-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f8007-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f8007-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8007-189">The publishing state for the app.</span></span> <span data-ttu-id="f8007-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f8007-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f8007-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8007-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f8007-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f8007-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f8007-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f8007-193">isAssigned</span></span>|<span data-ttu-id="f8007-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8007-194">Boolean</span></span>|<span data-ttu-id="f8007-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f8007-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f8007-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8007-197">roleScopeTagIds</span></span>|<span data-ttu-id="f8007-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8007-198">String collection</span></span>|<span data-ttu-id="f8007-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f8007-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f8007-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8007-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f8007-201">committedContentVersion</span></span>|<span data-ttu-id="f8007-202">String</span><span class="sxs-lookup"><span data-stu-id="f8007-202">String</span></span>|<span data-ttu-id="f8007-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f8007-203">The internal committed content version.</span></span> <span data-ttu-id="f8007-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f8007-205">fileName</span><span class="sxs-lookup"><span data-stu-id="f8007-205">fileName</span></span>|<span data-ttu-id="f8007-206">String</span><span class="sxs-lookup"><span data-stu-id="f8007-206">String</span></span>|<span data-ttu-id="f8007-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f8007-207">The name of the main Lob application file.</span></span> <span data-ttu-id="f8007-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f8007-209">size</span><span class="sxs-lookup"><span data-stu-id="f8007-209">size</span></span>|<span data-ttu-id="f8007-210">Int64</span><span class="sxs-lookup"><span data-stu-id="f8007-210">Int64</span></span>|<span data-ttu-id="f8007-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f8007-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="f8007-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8007-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f8007-213">packageId</span><span class="sxs-lookup"><span data-stu-id="f8007-213">packageId</span></span>|<span data-ttu-id="f8007-214">String</span><span class="sxs-lookup"><span data-stu-id="f8007-214">String</span></span>|<span data-ttu-id="f8007-215">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="f8007-215">The package identifier.</span></span>|
|<span data-ttu-id="f8007-216">identityName</span><span class="sxs-lookup"><span data-stu-id="f8007-216">identityName</span></span>|<span data-ttu-id="f8007-217">String</span><span class="sxs-lookup"><span data-stu-id="f8007-217">String</span></span>|<span data-ttu-id="f8007-218">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f8007-218">The Identity Name.</span></span>|
|<span data-ttu-id="f8007-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f8007-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f8007-220">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f8007-220">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f8007-221">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f8007-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f8007-222">versionName</span><span class="sxs-lookup"><span data-stu-id="f8007-222">versionName</span></span>|<span data-ttu-id="f8007-223">String</span><span class="sxs-lookup"><span data-stu-id="f8007-223">String</span></span>|<span data-ttu-id="f8007-224">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="f8007-224">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f8007-225">versionCode</span><span class="sxs-lookup"><span data-stu-id="f8007-225">versionCode</span></span>|<span data-ttu-id="f8007-226">String</span><span class="sxs-lookup"><span data-stu-id="f8007-226">String</span></span>|<span data-ttu-id="f8007-227">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="f8007-227">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f8007-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f8007-228">identityVersion</span></span>|<span data-ttu-id="f8007-229">String</span><span class="sxs-lookup"><span data-stu-id="f8007-229">String</span></span>|<span data-ttu-id="f8007-230">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f8007-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f8007-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8007-231">Response</span></span>
<span data-ttu-id="f8007-232">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8007-232">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8007-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8007-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8007-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8007-234">Request</span></span>
<span data-ttu-id="f8007-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8007-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1386

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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

### <a name="response"></a><span data-ttu-id="f8007-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8007-236">Response</span></span>
<span data-ttu-id="f8007-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8007-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1558

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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




