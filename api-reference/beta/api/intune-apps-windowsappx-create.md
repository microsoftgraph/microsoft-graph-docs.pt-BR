---
title: Criar windowsAppX
description: Criar um novo objeto windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12854a2bcb5668634eef96a4063a857d460a455a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791544"
---
# <a name="create-windowsappx"></a><span data-ttu-id="fb350-103">Criar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="fb350-103">Create windowsAppX</span></span>

<span data-ttu-id="fb350-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb350-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb350-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb350-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb350-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb350-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb350-107">Criar um novo objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="fb350-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb350-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb350-108">Prerequisites</span></span>
<span data-ttu-id="fb350-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb350-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb350-111">Permission type</span></span>|<span data-ttu-id="fb350-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb350-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb350-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb350-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb350-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb350-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb350-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb350-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb350-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb350-116">Not supported.</span></span>|
|<span data-ttu-id="fb350-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb350-117">Application</span></span>|<span data-ttu-id="fb350-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb350-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb350-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb350-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fb350-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb350-120">Request headers</span></span>
|<span data-ttu-id="fb350-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb350-121">Header</span></span>|<span data-ttu-id="fb350-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fb350-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb350-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb350-123">Authorization</span></span>|<span data-ttu-id="fb350-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb350-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb350-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb350-125">Accept</span></span>|<span data-ttu-id="fb350-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb350-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb350-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb350-127">Request body</span></span>
<span data-ttu-id="fb350-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="fb350-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="fb350-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="fb350-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="fb350-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb350-130">Property</span></span>|<span data-ttu-id="fb350-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb350-131">Type</span></span>|<span data-ttu-id="fb350-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb350-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb350-133">id</span><span class="sxs-lookup"><span data-stu-id="fb350-133">id</span></span>|<span data-ttu-id="fb350-134">String</span><span class="sxs-lookup"><span data-stu-id="fb350-134">String</span></span>|<span data-ttu-id="fb350-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fb350-135">Key of the entity.</span></span> <span data-ttu-id="fb350-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fb350-137">displayName</span></span>|<span data-ttu-id="fb350-138">String</span><span class="sxs-lookup"><span data-stu-id="fb350-138">String</span></span>|<span data-ttu-id="fb350-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fb350-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fb350-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-141">description</span><span class="sxs-lookup"><span data-stu-id="fb350-141">description</span></span>|<span data-ttu-id="fb350-142">String</span><span class="sxs-lookup"><span data-stu-id="fb350-142">String</span></span>|<span data-ttu-id="fb350-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb350-143">The description of the app.</span></span> <span data-ttu-id="fb350-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-145">publicador</span><span class="sxs-lookup"><span data-stu-id="fb350-145">publisher</span></span>|<span data-ttu-id="fb350-146">String</span><span class="sxs-lookup"><span data-stu-id="fb350-146">String</span></span>|<span data-ttu-id="fb350-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb350-147">The publisher of the app.</span></span> <span data-ttu-id="fb350-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fb350-149">largeIcon</span></span>|[<span data-ttu-id="fb350-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb350-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fb350-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="fb350-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fb350-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb350-153">createdDateTime</span></span>|<span data-ttu-id="fb350-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb350-154">DateTimeOffset</span></span>|<span data-ttu-id="fb350-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb350-155">The date and time the app was created.</span></span> <span data-ttu-id="fb350-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb350-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fb350-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb350-158">DateTimeOffset</span></span>|<span data-ttu-id="fb350-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fb350-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fb350-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fb350-161">isFeatured</span></span>|<span data-ttu-id="fb350-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb350-162">Boolean</span></span>|<span data-ttu-id="fb350-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fb350-164">privacyInformationUrl</span></span>|<span data-ttu-id="fb350-165">String</span><span class="sxs-lookup"><span data-stu-id="fb350-165">String</span></span>|<span data-ttu-id="fb350-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fb350-166">The privacy statement Url.</span></span> <span data-ttu-id="fb350-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fb350-168">informationUrl</span></span>|<span data-ttu-id="fb350-169">String</span><span class="sxs-lookup"><span data-stu-id="fb350-169">String</span></span>|<span data-ttu-id="fb350-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fb350-170">The more information Url.</span></span> <span data-ttu-id="fb350-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-172">owner</span><span class="sxs-lookup"><span data-stu-id="fb350-172">owner</span></span>|<span data-ttu-id="fb350-173">String</span><span class="sxs-lookup"><span data-stu-id="fb350-173">String</span></span>|<span data-ttu-id="fb350-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fb350-174">The owner of the app.</span></span> <span data-ttu-id="fb350-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-176">developer</span><span class="sxs-lookup"><span data-stu-id="fb350-176">developer</span></span>|<span data-ttu-id="fb350-177">String</span><span class="sxs-lookup"><span data-stu-id="fb350-177">String</span></span>|<span data-ttu-id="fb350-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb350-178">The developer of the app.</span></span> <span data-ttu-id="fb350-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-180">notes</span><span class="sxs-lookup"><span data-stu-id="fb350-180">notes</span></span>|<span data-ttu-id="fb350-181">String</span><span class="sxs-lookup"><span data-stu-id="fb350-181">String</span></span>|<span data-ttu-id="fb350-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb350-182">Notes for the app.</span></span> <span data-ttu-id="fb350-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fb350-184">uploadState</span></span>|<span data-ttu-id="fb350-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fb350-185">Int32</span></span>|<span data-ttu-id="fb350-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="fb350-186">The upload state.</span></span> <span data-ttu-id="fb350-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="fb350-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="fb350-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="fb350-189">publishingState</span></span>|[<span data-ttu-id="fb350-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fb350-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fb350-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb350-191">The publishing state for the app.</span></span> <span data-ttu-id="fb350-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="fb350-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fb350-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb350-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="fb350-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fb350-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fb350-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fb350-195">isAssigned</span></span>|<span data-ttu-id="fb350-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb350-196">Boolean</span></span>|<span data-ttu-id="fb350-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="fb350-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fb350-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb350-199">roleScopeTagIds</span></span>|<span data-ttu-id="fb350-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb350-200">String collection</span></span>|<span data-ttu-id="fb350-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="fb350-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fb350-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="fb350-203">dependentAppCount</span></span>|<span data-ttu-id="fb350-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fb350-204">Int32</span></span>|<span data-ttu-id="fb350-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="fb350-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fb350-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb350-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fb350-207">committedContentVersion</span></span>|<span data-ttu-id="fb350-208">String</span><span class="sxs-lookup"><span data-stu-id="fb350-208">String</span></span>|<span data-ttu-id="fb350-209">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="fb350-209">The internal committed content version.</span></span> <span data-ttu-id="fb350-210">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb350-211">fileName</span><span class="sxs-lookup"><span data-stu-id="fb350-211">fileName</span></span>|<span data-ttu-id="fb350-212">String</span><span class="sxs-lookup"><span data-stu-id="fb350-212">String</span></span>|<span data-ttu-id="fb350-213">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="fb350-213">The name of the main Lob application file.</span></span> <span data-ttu-id="fb350-214">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb350-215">size</span><span class="sxs-lookup"><span data-stu-id="fb350-215">size</span></span>|<span data-ttu-id="fb350-216">Int64</span><span class="sxs-lookup"><span data-stu-id="fb350-216">Int64</span></span>|<span data-ttu-id="fb350-217">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="fb350-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="fb350-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb350-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb350-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="fb350-219">applicableArchitectures</span></span>|[<span data-ttu-id="fb350-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="fb350-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="fb350-221">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="fb350-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="fb350-222">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="fb350-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="fb350-223">identityName</span><span class="sxs-lookup"><span data-stu-id="fb350-223">identityName</span></span>|<span data-ttu-id="fb350-224">String</span><span class="sxs-lookup"><span data-stu-id="fb350-224">String</span></span>|<span data-ttu-id="fb350-225">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="fb350-225">The Identity Name.</span></span>|
|<span data-ttu-id="fb350-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="fb350-226">identityPublisherHash</span></span>|<span data-ttu-id="fb350-227">String</span><span class="sxs-lookup"><span data-stu-id="fb350-227">String</span></span>|<span data-ttu-id="fb350-228">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="fb350-228">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="fb350-229">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb350-229">identityResourceIdentifier</span></span>|<span data-ttu-id="fb350-230">String</span><span class="sxs-lookup"><span data-stu-id="fb350-230">String</span></span>|<span data-ttu-id="fb350-231">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="fb350-231">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="fb350-232">isBundle</span><span class="sxs-lookup"><span data-stu-id="fb350-232">isBundle</span></span>|<span data-ttu-id="fb350-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb350-233">Boolean</span></span>|<span data-ttu-id="fb350-234">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="fb350-234">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="fb350-235">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb350-235">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fb350-236">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb350-236">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="fb350-237">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="fb350-237">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fb350-238">identityVersion</span><span class="sxs-lookup"><span data-stu-id="fb350-238">identityVersion</span></span>|<span data-ttu-id="fb350-239">String</span><span class="sxs-lookup"><span data-stu-id="fb350-239">String</span></span>|<span data-ttu-id="fb350-240">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="fb350-240">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="fb350-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb350-241">Response</span></span>
<span data-ttu-id="fb350-242">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb350-242">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb350-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb350-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb350-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb350-244">Request</span></span>
<span data-ttu-id="fb350-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb350-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1413

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
  "dependentAppCount": 1,
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="fb350-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb350-246">Response</span></span>
<span data-ttu-id="fb350-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb350-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1585

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
  "dependentAppCount": 1,
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```



