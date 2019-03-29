---
title: Criar windowsAppX
description: Criar um novo objeto windowsAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1472de7e4db226570e599072f541a3e1884de2a6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961249"
---
# <a name="create-windowsappx"></a><span data-ttu-id="faa60-103">Criar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="faa60-103">Create windowsAppX</span></span>

> <span data-ttu-id="faa60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="faa60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faa60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="faa60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa60-106">Criar um novo objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="faa60-106">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faa60-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="faa60-107">Prerequisites</span></span>
<span data-ttu-id="faa60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faa60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faa60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="faa60-110">Permission type</span></span>|<span data-ttu-id="faa60-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="faa60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faa60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faa60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="faa60-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa60-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="faa60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faa60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faa60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faa60-115">Not supported.</span></span>|
|<span data-ttu-id="faa60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faa60-116">Application</span></span>|<span data-ttu-id="faa60-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faa60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faa60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faa60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="faa60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faa60-119">Request headers</span></span>
|<span data-ttu-id="faa60-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="faa60-120">Header</span></span>|<span data-ttu-id="faa60-121">Valor</span><span class="sxs-lookup"><span data-stu-id="faa60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faa60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="faa60-122">Authorization</span></span>|<span data-ttu-id="faa60-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faa60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faa60-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="faa60-124">Accept</span></span>|<span data-ttu-id="faa60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="faa60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faa60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faa60-126">Request body</span></span>
<span data-ttu-id="faa60-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="faa60-127">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="faa60-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="faa60-128">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="faa60-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faa60-129">Property</span></span>|<span data-ttu-id="faa60-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="faa60-130">Type</span></span>|<span data-ttu-id="faa60-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa60-132">id</span><span class="sxs-lookup"><span data-stu-id="faa60-132">id</span></span>|<span data-ttu-id="faa60-133">String</span><span class="sxs-lookup"><span data-stu-id="faa60-133">String</span></span>|<span data-ttu-id="faa60-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="faa60-134">Key of the entity.</span></span> <span data-ttu-id="faa60-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-136">displayName</span><span class="sxs-lookup"><span data-stu-id="faa60-136">displayName</span></span>|<span data-ttu-id="faa60-137">String</span><span class="sxs-lookup"><span data-stu-id="faa60-137">String</span></span>|<span data-ttu-id="faa60-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="faa60-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="faa60-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-140">descrição</span><span class="sxs-lookup"><span data-stu-id="faa60-140">description</span></span>|<span data-ttu-id="faa60-141">String</span><span class="sxs-lookup"><span data-stu-id="faa60-141">String</span></span>|<span data-ttu-id="faa60-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="faa60-142">The description of the app.</span></span> <span data-ttu-id="faa60-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-144">publicador</span><span class="sxs-lookup"><span data-stu-id="faa60-144">publisher</span></span>|<span data-ttu-id="faa60-145">String</span><span class="sxs-lookup"><span data-stu-id="faa60-145">String</span></span>|<span data-ttu-id="faa60-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="faa60-146">The publisher of the app.</span></span> <span data-ttu-id="faa60-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="faa60-148">largeIcon</span></span>|[<span data-ttu-id="faa60-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="faa60-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="faa60-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="faa60-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="faa60-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faa60-152">createdDateTime</span></span>|<span data-ttu-id="faa60-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faa60-153">DateTimeOffset</span></span>|<span data-ttu-id="faa60-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="faa60-154">The date and time the app was created.</span></span> <span data-ttu-id="faa60-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faa60-156">lastModifiedDateTime</span></span>|<span data-ttu-id="faa60-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faa60-157">DateTimeOffset</span></span>|<span data-ttu-id="faa60-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="faa60-158">The date and time the app was last modified.</span></span> <span data-ttu-id="faa60-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="faa60-160">isFeatured</span></span>|<span data-ttu-id="faa60-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa60-161">Boolean</span></span>|<span data-ttu-id="faa60-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="faa60-163">privacyInformationUrl</span></span>|<span data-ttu-id="faa60-164">String</span><span class="sxs-lookup"><span data-stu-id="faa60-164">String</span></span>|<span data-ttu-id="faa60-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="faa60-165">The privacy statement Url.</span></span> <span data-ttu-id="faa60-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="faa60-167">informationUrl</span></span>|<span data-ttu-id="faa60-168">String</span><span class="sxs-lookup"><span data-stu-id="faa60-168">String</span></span>|<span data-ttu-id="faa60-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="faa60-169">The more information Url.</span></span> <span data-ttu-id="faa60-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-171">owner</span><span class="sxs-lookup"><span data-stu-id="faa60-171">owner</span></span>|<span data-ttu-id="faa60-172">String</span><span class="sxs-lookup"><span data-stu-id="faa60-172">String</span></span>|<span data-ttu-id="faa60-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="faa60-173">The owner of the app.</span></span> <span data-ttu-id="faa60-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-175">developer</span><span class="sxs-lookup"><span data-stu-id="faa60-175">developer</span></span>|<span data-ttu-id="faa60-176">String</span><span class="sxs-lookup"><span data-stu-id="faa60-176">String</span></span>|<span data-ttu-id="faa60-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="faa60-177">The developer of the app.</span></span> <span data-ttu-id="faa60-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-179">notes</span><span class="sxs-lookup"><span data-stu-id="faa60-179">notes</span></span>|<span data-ttu-id="faa60-180">String</span><span class="sxs-lookup"><span data-stu-id="faa60-180">String</span></span>|<span data-ttu-id="faa60-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="faa60-181">Notes for the app.</span></span> <span data-ttu-id="faa60-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="faa60-183">uploadState</span></span>|<span data-ttu-id="faa60-184">Int32</span><span class="sxs-lookup"><span data-stu-id="faa60-184">Int32</span></span>|<span data-ttu-id="faa60-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="faa60-185">The upload state.</span></span> <span data-ttu-id="faa60-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="faa60-187">publishingState</span></span>|[<span data-ttu-id="faa60-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="faa60-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="faa60-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="faa60-189">The publishing state for the app.</span></span> <span data-ttu-id="faa60-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="faa60-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="faa60-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="faa60-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="faa60-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="faa60-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="faa60-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="faa60-193">isAssigned</span></span>|<span data-ttu-id="faa60-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa60-194">Boolean</span></span>|<span data-ttu-id="faa60-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="faa60-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="faa60-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="faa60-197">roleScopeTagIds</span></span>|<span data-ttu-id="faa60-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="faa60-198">String collection</span></span>|<span data-ttu-id="faa60-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="faa60-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="faa60-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="faa60-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="faa60-201">committedContentVersion</span></span>|<span data-ttu-id="faa60-202">String</span><span class="sxs-lookup"><span data-stu-id="faa60-202">String</span></span>|<span data-ttu-id="faa60-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="faa60-203">The internal committed content version.</span></span> <span data-ttu-id="faa60-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="faa60-205">fileName</span><span class="sxs-lookup"><span data-stu-id="faa60-205">fileName</span></span>|<span data-ttu-id="faa60-206">String</span><span class="sxs-lookup"><span data-stu-id="faa60-206">String</span></span>|<span data-ttu-id="faa60-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="faa60-207">The name of the main Lob application file.</span></span> <span data-ttu-id="faa60-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="faa60-209">size</span><span class="sxs-lookup"><span data-stu-id="faa60-209">size</span></span>|<span data-ttu-id="faa60-210">Int64</span><span class="sxs-lookup"><span data-stu-id="faa60-210">Int64</span></span>|<span data-ttu-id="faa60-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="faa60-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="faa60-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="faa60-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="faa60-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="faa60-213">applicableArchitectures</span></span>|[<span data-ttu-id="faa60-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="faa60-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="faa60-215">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="faa60-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="faa60-216">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="faa60-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="faa60-217">identityName</span><span class="sxs-lookup"><span data-stu-id="faa60-217">identityName</span></span>|<span data-ttu-id="faa60-218">String</span><span class="sxs-lookup"><span data-stu-id="faa60-218">String</span></span>|<span data-ttu-id="faa60-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="faa60-219">The Identity Name.</span></span>|
|<span data-ttu-id="faa60-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="faa60-220">identityPublisherHash</span></span>|<span data-ttu-id="faa60-221">String</span><span class="sxs-lookup"><span data-stu-id="faa60-221">String</span></span>|<span data-ttu-id="faa60-222">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="faa60-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="faa60-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="faa60-223">identityResourceIdentifier</span></span>|<span data-ttu-id="faa60-224">String</span><span class="sxs-lookup"><span data-stu-id="faa60-224">String</span></span>|<span data-ttu-id="faa60-225">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="faa60-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="faa60-226">isBundle</span><span class="sxs-lookup"><span data-stu-id="faa60-226">isBundle</span></span>|<span data-ttu-id="faa60-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa60-227">Boolean</span></span>|<span data-ttu-id="faa60-228">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="faa60-228">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="faa60-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="faa60-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="faa60-230">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="faa60-230">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="faa60-231">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="faa60-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="faa60-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="faa60-232">identityVersion</span></span>|<span data-ttu-id="faa60-233">String</span><span class="sxs-lookup"><span data-stu-id="faa60-233">String</span></span>|<span data-ttu-id="faa60-234">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="faa60-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="faa60-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="faa60-235">Response</span></span>
<span data-ttu-id="faa60-236">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faa60-236">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faa60-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faa60-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="faa60-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faa60-238">Request</span></span>
<span data-ttu-id="faa60-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="faa60-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="faa60-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="faa60-240">Response</span></span>
<span data-ttu-id="faa60-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="faa60-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1512

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```




