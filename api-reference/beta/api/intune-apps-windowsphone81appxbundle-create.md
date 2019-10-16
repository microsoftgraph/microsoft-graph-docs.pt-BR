---
title: Criar windowsPhone81AppXBundle
description: Criar um novo objeto windowsPhone81AppXBundle.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f751464acf0421de7fb32a71d71845d8ec9aef03
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535020"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="b75cf-103">Criar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="b75cf-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="b75cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b75cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b75cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b75cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b75cf-106">Criar um novo objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="b75cf-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b75cf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b75cf-107">Prerequisites</span></span>
<span data-ttu-id="b75cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b75cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b75cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b75cf-110">Permission type</span></span>|<span data-ttu-id="b75cf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b75cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b75cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b75cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b75cf-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b75cf-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b75cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b75cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b75cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b75cf-115">Not supported.</span></span>|
|<span data-ttu-id="b75cf-116">Application</span><span class="sxs-lookup"><span data-stu-id="b75cf-116">Application</span></span>|<span data-ttu-id="b75cf-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b75cf-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b75cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b75cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b75cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b75cf-119">Request headers</span></span>
|<span data-ttu-id="b75cf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b75cf-120">Header</span></span>|<span data-ttu-id="b75cf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b75cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b75cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b75cf-122">Authorization</span></span>|<span data-ttu-id="b75cf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b75cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b75cf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b75cf-124">Accept</span></span>|<span data-ttu-id="b75cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b75cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b75cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b75cf-126">Request body</span></span>
<span data-ttu-id="b75cf-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="b75cf-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="b75cf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="b75cf-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="b75cf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b75cf-129">Property</span></span>|<span data-ttu-id="b75cf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b75cf-130">Type</span></span>|<span data-ttu-id="b75cf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b75cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b75cf-132">id</span><span class="sxs-lookup"><span data-stu-id="b75cf-132">id</span></span>|<span data-ttu-id="b75cf-133">String</span><span class="sxs-lookup"><span data-stu-id="b75cf-133">String</span></span>|<span data-ttu-id="b75cf-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b75cf-134">Key of the entity.</span></span> <span data-ttu-id="b75cf-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b75cf-136">displayName</span></span>|<span data-ttu-id="b75cf-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-137">String</span></span>|<span data-ttu-id="b75cf-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b75cf-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b75cf-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-140">description</span><span class="sxs-lookup"><span data-stu-id="b75cf-140">description</span></span>|<span data-ttu-id="b75cf-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-141">String</span></span>|<span data-ttu-id="b75cf-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-142">The description of the app.</span></span> <span data-ttu-id="b75cf-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-144">publicador</span><span class="sxs-lookup"><span data-stu-id="b75cf-144">publisher</span></span>|<span data-ttu-id="b75cf-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-145">String</span></span>|<span data-ttu-id="b75cf-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-146">The publisher of the app.</span></span> <span data-ttu-id="b75cf-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b75cf-148">largeIcon</span></span>|[<span data-ttu-id="b75cf-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b75cf-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b75cf-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b75cf-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b75cf-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b75cf-152">createdDateTime</span></span>|<span data-ttu-id="b75cf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75cf-153">DateTimeOffset</span></span>|<span data-ttu-id="b75cf-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-154">The date and time the app was created.</span></span> <span data-ttu-id="b75cf-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b75cf-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b75cf-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75cf-157">DateTimeOffset</span></span>|<span data-ttu-id="b75cf-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b75cf-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b75cf-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b75cf-160">isFeatured</span></span>|<span data-ttu-id="b75cf-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b75cf-161">Boolean</span></span>|<span data-ttu-id="b75cf-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b75cf-163">privacyInformationUrl</span></span>|<span data-ttu-id="b75cf-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-164">String</span></span>|<span data-ttu-id="b75cf-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b75cf-165">The privacy statement Url.</span></span> <span data-ttu-id="b75cf-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b75cf-167">informationUrl</span></span>|<span data-ttu-id="b75cf-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-168">String</span></span>|<span data-ttu-id="b75cf-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b75cf-169">The more information Url.</span></span> <span data-ttu-id="b75cf-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-171">owner</span><span class="sxs-lookup"><span data-stu-id="b75cf-171">owner</span></span>|<span data-ttu-id="b75cf-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-172">String</span></span>|<span data-ttu-id="b75cf-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-173">The owner of the app.</span></span> <span data-ttu-id="b75cf-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-175">developer</span><span class="sxs-lookup"><span data-stu-id="b75cf-175">developer</span></span>|<span data-ttu-id="b75cf-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-176">String</span></span>|<span data-ttu-id="b75cf-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-177">The developer of the app.</span></span> <span data-ttu-id="b75cf-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-179">notes</span><span class="sxs-lookup"><span data-stu-id="b75cf-179">notes</span></span>|<span data-ttu-id="b75cf-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-180">String</span></span>|<span data-ttu-id="b75cf-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-181">Notes for the app.</span></span> <span data-ttu-id="b75cf-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b75cf-183">uploadState</span></span>|<span data-ttu-id="b75cf-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b75cf-184">Int32</span></span>|<span data-ttu-id="b75cf-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="b75cf-185">The upload state.</span></span> <span data-ttu-id="b75cf-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b75cf-187">publishingState</span></span>|[<span data-ttu-id="b75cf-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b75cf-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b75cf-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-189">The publishing state for the app.</span></span> <span data-ttu-id="b75cf-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b75cf-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b75cf-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b75cf-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b75cf-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b75cf-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b75cf-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b75cf-193">isAssigned</span></span>|<span data-ttu-id="b75cf-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b75cf-194">Boolean</span></span>|<span data-ttu-id="b75cf-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="b75cf-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b75cf-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b75cf-197">roleScopeTagIds</span></span>|<span data-ttu-id="b75cf-198">String collection</span><span class="sxs-lookup"><span data-stu-id="b75cf-198">String collection</span></span>|<span data-ttu-id="b75cf-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b75cf-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b75cf-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b75cf-201">dependentAppCount</span></span>|<span data-ttu-id="b75cf-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b75cf-202">Int32</span></span>|<span data-ttu-id="b75cf-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="b75cf-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b75cf-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b75cf-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b75cf-205">committedContentVersion</span></span>|<span data-ttu-id="b75cf-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-206">String</span></span>|<span data-ttu-id="b75cf-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="b75cf-207">The internal committed content version.</span></span> <span data-ttu-id="b75cf-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b75cf-209">fileName</span><span class="sxs-lookup"><span data-stu-id="b75cf-209">fileName</span></span>|<span data-ttu-id="b75cf-210">String</span><span class="sxs-lookup"><span data-stu-id="b75cf-210">String</span></span>|<span data-ttu-id="b75cf-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="b75cf-211">The name of the main Lob application file.</span></span> <span data-ttu-id="b75cf-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b75cf-213">size</span><span class="sxs-lookup"><span data-stu-id="b75cf-213">size</span></span>|<span data-ttu-id="b75cf-214">Int64</span><span class="sxs-lookup"><span data-stu-id="b75cf-214">Int64</span></span>|<span data-ttu-id="b75cf-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="b75cf-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="b75cf-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b75cf-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b75cf-217">applicableArchitectures</span></span>|[<span data-ttu-id="b75cf-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b75cf-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b75cf-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b75cf-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b75cf-220">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="b75cf-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="b75cf-221">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="b75cf-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b75cf-222">identityName</span><span class="sxs-lookup"><span data-stu-id="b75cf-222">identityName</span></span>|<span data-ttu-id="b75cf-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-223">String</span></span>|<span data-ttu-id="b75cf-224">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b75cf-224">The Identity Name.</span></span> <span data-ttu-id="b75cf-225">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b75cf-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="b75cf-226">identityPublisherHash</span></span>|<span data-ttu-id="b75cf-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-227">String</span></span>|<span data-ttu-id="b75cf-228">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="b75cf-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="b75cf-229">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b75cf-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b75cf-230">identityResourceIdentifier</span></span>|<span data-ttu-id="b75cf-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-231">String</span></span>|<span data-ttu-id="b75cf-232">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b75cf-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="b75cf-233">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b75cf-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b75cf-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b75cf-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b75cf-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b75cf-236">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b75cf-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="b75cf-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b75cf-238">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="b75cf-238">phoneProductIdentifier</span></span>|<span data-ttu-id="b75cf-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-239">String</span></span>|<span data-ttu-id="b75cf-240">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="b75cf-240">The Phone Product Identifier.</span></span> <span data-ttu-id="b75cf-241">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b75cf-242">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="b75cf-242">phonePublisherId</span></span>|<span data-ttu-id="b75cf-243">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75cf-243">String</span></span>|<span data-ttu-id="b75cf-244">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b75cf-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b75cf-245">identityVersion</span></span>|<span data-ttu-id="b75cf-246">String</span><span class="sxs-lookup"><span data-stu-id="b75cf-246">String</span></span>|<span data-ttu-id="b75cf-247">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="b75cf-247">The identity version.</span></span> <span data-ttu-id="b75cf-248">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b75cf-249">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="b75cf-249">appXPackageInformationList</span></span>|<span data-ttu-id="b75cf-250">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="b75cf-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="b75cf-251">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="b75cf-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="b75cf-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="b75cf-252">Response</span></span>
<span data-ttu-id="b75cf-253">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b75cf-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b75cf-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b75cf-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="b75cf-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b75cf-255">Request</span></span>
<span data-ttu-id="b75cf-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b75cf-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2311

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b75cf-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="b75cf-257">Response</span></span>
<span data-ttu-id="b75cf-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b75cf-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2483

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```






