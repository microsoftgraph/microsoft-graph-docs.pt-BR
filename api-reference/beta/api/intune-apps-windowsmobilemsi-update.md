---
title: Atualizar windowsMobileMSI
description: Atualiza as propriedades de um objeto windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53cbb26a41ad6c8281f95c114e00d76eeb20aa91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393673"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="4e22c-103">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="4e22c-103">Update windowsMobileMSI</span></span>

<span data-ttu-id="4e22c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e22c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e22c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e22c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e22c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e22c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e22c-107">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="4e22c-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e22c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e22c-108">Prerequisites</span></span>
<span data-ttu-id="4e22c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e22c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e22c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e22c-111">Permission type</span></span>|<span data-ttu-id="4e22c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e22c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e22c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e22c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e22c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e22c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e22c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e22c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e22c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e22c-116">Not supported.</span></span>|
|<span data-ttu-id="4e22c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e22c-117">Application</span></span>|<span data-ttu-id="4e22c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e22c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e22c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e22c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4e22c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e22c-120">Request headers</span></span>
|<span data-ttu-id="4e22c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e22c-121">Header</span></span>|<span data-ttu-id="4e22c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4e22c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e22c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e22c-123">Authorization</span></span>|<span data-ttu-id="4e22c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e22c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e22c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e22c-125">Accept</span></span>|<span data-ttu-id="4e22c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e22c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e22c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e22c-127">Request body</span></span>
<span data-ttu-id="4e22c-128">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="4e22c-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="4e22c-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="4e22c-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="4e22c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e22c-130">Property</span></span>|<span data-ttu-id="4e22c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e22c-131">Type</span></span>|<span data-ttu-id="4e22c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e22c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e22c-133">id</span><span class="sxs-lookup"><span data-stu-id="4e22c-133">id</span></span>|<span data-ttu-id="4e22c-134">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-134">String</span></span>|<span data-ttu-id="4e22c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e22c-135">Key of the entity.</span></span> <span data-ttu-id="4e22c-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4e22c-137">displayName</span></span>|<span data-ttu-id="4e22c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e22c-138">String</span></span>|<span data-ttu-id="4e22c-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4e22c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4e22c-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-141">description</span><span class="sxs-lookup"><span data-stu-id="4e22c-141">description</span></span>|<span data-ttu-id="4e22c-142">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-142">String</span></span>|<span data-ttu-id="4e22c-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-143">The description of the app.</span></span> <span data-ttu-id="4e22c-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-145">publicador</span><span class="sxs-lookup"><span data-stu-id="4e22c-145">publisher</span></span>|<span data-ttu-id="4e22c-146">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-146">String</span></span>|<span data-ttu-id="4e22c-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-147">The publisher of the app.</span></span> <span data-ttu-id="4e22c-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4e22c-149">largeIcon</span></span>|[<span data-ttu-id="4e22c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4e22c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4e22c-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4e22c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4e22c-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e22c-153">createdDateTime</span></span>|<span data-ttu-id="4e22c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e22c-154">DateTimeOffset</span></span>|<span data-ttu-id="4e22c-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-155">The date and time the app was created.</span></span> <span data-ttu-id="4e22c-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e22c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4e22c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e22c-158">DateTimeOffset</span></span>|<span data-ttu-id="4e22c-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4e22c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4e22c-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4e22c-161">isFeatured</span></span>|<span data-ttu-id="4e22c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e22c-162">Boolean</span></span>|<span data-ttu-id="4e22c-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4e22c-164">privacyInformationUrl</span></span>|<span data-ttu-id="4e22c-165">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-165">String</span></span>|<span data-ttu-id="4e22c-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4e22c-166">The privacy statement Url.</span></span> <span data-ttu-id="4e22c-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4e22c-168">informationUrl</span></span>|<span data-ttu-id="4e22c-169">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-169">String</span></span>|<span data-ttu-id="4e22c-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4e22c-170">The more information Url.</span></span> <span data-ttu-id="4e22c-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-172">owner</span><span class="sxs-lookup"><span data-stu-id="4e22c-172">owner</span></span>|<span data-ttu-id="4e22c-173">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-173">String</span></span>|<span data-ttu-id="4e22c-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-174">The owner of the app.</span></span> <span data-ttu-id="4e22c-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-176">developer</span><span class="sxs-lookup"><span data-stu-id="4e22c-176">developer</span></span>|<span data-ttu-id="4e22c-177">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-177">String</span></span>|<span data-ttu-id="4e22c-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-178">The developer of the app.</span></span> <span data-ttu-id="4e22c-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-180">notes</span><span class="sxs-lookup"><span data-stu-id="4e22c-180">notes</span></span>|<span data-ttu-id="4e22c-181">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-181">String</span></span>|<span data-ttu-id="4e22c-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-182">Notes for the app.</span></span> <span data-ttu-id="4e22c-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4e22c-184">uploadState</span></span>|<span data-ttu-id="4e22c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4e22c-185">Int32</span></span>|<span data-ttu-id="4e22c-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="4e22c-186">The upload state.</span></span> <span data-ttu-id="4e22c-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4e22c-188">publishingState</span></span>|[<span data-ttu-id="4e22c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4e22c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4e22c-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-190">The publishing state for the app.</span></span> <span data-ttu-id="4e22c-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4e22c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4e22c-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e22c-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4e22c-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4e22c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4e22c-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4e22c-194">isAssigned</span></span>|<span data-ttu-id="4e22c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e22c-195">Boolean</span></span>|<span data-ttu-id="4e22c-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4e22c-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e22c-198">roleScopeTagIds</span></span>|<span data-ttu-id="4e22c-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4e22c-199">String collection</span></span>|<span data-ttu-id="4e22c-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4e22c-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4e22c-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4e22c-202">dependentAppCount</span></span>|<span data-ttu-id="4e22c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="4e22c-203">Int32</span></span>|<span data-ttu-id="4e22c-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="4e22c-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4e22c-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e22c-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4e22c-206">committedContentVersion</span></span>|<span data-ttu-id="4e22c-207">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-207">String</span></span>|<span data-ttu-id="4e22c-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="4e22c-208">The internal committed content version.</span></span> <span data-ttu-id="4e22c-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4e22c-210">fileName</span><span class="sxs-lookup"><span data-stu-id="4e22c-210">fileName</span></span>|<span data-ttu-id="4e22c-211">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-211">String</span></span>|<span data-ttu-id="4e22c-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="4e22c-212">The name of the main Lob application file.</span></span> <span data-ttu-id="4e22c-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4e22c-214">size</span><span class="sxs-lookup"><span data-stu-id="4e22c-214">size</span></span>|<span data-ttu-id="4e22c-215">Int64</span><span class="sxs-lookup"><span data-stu-id="4e22c-215">Int64</span></span>|<span data-ttu-id="4e22c-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="4e22c-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="4e22c-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e22c-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4e22c-218">commandLine</span><span class="sxs-lookup"><span data-stu-id="4e22c-218">commandLine</span></span>|<span data-ttu-id="4e22c-219">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-219">String</span></span>|<span data-ttu-id="4e22c-220">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="4e22c-220">The command line.</span></span>|
|<span data-ttu-id="4e22c-221">productCode</span><span class="sxs-lookup"><span data-stu-id="4e22c-221">productCode</span></span>|<span data-ttu-id="4e22c-222">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-222">String</span></span>|<span data-ttu-id="4e22c-223">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="4e22c-223">The product code.</span></span>|
|<span data-ttu-id="4e22c-224">productVersion</span><span class="sxs-lookup"><span data-stu-id="4e22c-224">productVersion</span></span>|<span data-ttu-id="4e22c-225">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-225">String</span></span>|<span data-ttu-id="4e22c-226">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="4e22c-226">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4e22c-227">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="4e22c-227">ignoreVersionDetection</span></span>|<span data-ttu-id="4e22c-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e22c-228">Boolean</span></span>|<span data-ttu-id="4e22c-229">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-229">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="4e22c-230">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="4e22c-230">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="4e22c-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4e22c-231">identityVersion</span></span>|<span data-ttu-id="4e22c-232">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-232">String</span></span>|<span data-ttu-id="4e22c-233">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="4e22c-233">The identity version.</span></span>|
|<span data-ttu-id="4e22c-234">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="4e22c-234">useDeviceContext</span></span>|<span data-ttu-id="4e22c-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e22c-235">Boolean</span></span>|<span data-ttu-id="4e22c-236">Indica se um MSI de modo duplo deve ser instalado no contexto de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-236">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="4e22c-237">Se true, o aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="4e22c-237">If true, app will be installed for all users.</span></span> <span data-ttu-id="4e22c-238">Se false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="4e22c-238">If false, app will be installed per-user.</span></span> <span data-ttu-id="4e22c-239">Se for NULL, o serviço usará o contexto de instalação padrão do pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="4e22c-239">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="4e22c-240">No caso do MSI de modo duplo, esse padrão será por usuário.</span><span class="sxs-lookup"><span data-stu-id="4e22c-240">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="4e22c-241">Não pode ser definido para aplicativos de modo não duplo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-241">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="4e22c-242">Não pode ser alterado após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4e22c-242">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="4e22c-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e22c-243">Response</span></span>
<span data-ttu-id="4e22c-244">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e22c-244">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e22c-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e22c-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e22c-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e22c-246">Request</span></span>
<span data-ttu-id="4e22c-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e22c-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1066

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="4e22c-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e22c-248">Response</span></span>
<span data-ttu-id="4e22c-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e22c-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1238

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```



