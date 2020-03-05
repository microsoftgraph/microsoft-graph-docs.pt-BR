---
title: Criar windowsPhone81AppXBundle
description: Criar um novo objeto windowsPhone81AppXBundle.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3edf8d2f87c77eeddaab16b3b738926d8ac79043
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450500"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="cefef-103">Criar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="cefef-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="cefef-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cefef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cefef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cefef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cefef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cefef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cefef-107">Criar um novo objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="cefef-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cefef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cefef-108">Prerequisites</span></span>
<span data-ttu-id="cefef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cefef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cefef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cefef-111">Permission type</span></span>|<span data-ttu-id="cefef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cefef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cefef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cefef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cefef-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefef-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cefef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cefef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cefef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cefef-116">Not supported.</span></span>|
|<span data-ttu-id="cefef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cefef-117">Application</span></span>|<span data-ttu-id="cefef-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefef-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cefef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cefef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cefef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cefef-120">Request headers</span></span>
|<span data-ttu-id="cefef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cefef-121">Header</span></span>|<span data-ttu-id="cefef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cefef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cefef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cefef-123">Authorization</span></span>|<span data-ttu-id="cefef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cefef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cefef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cefef-125">Accept</span></span>|<span data-ttu-id="cefef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cefef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cefef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cefef-127">Request body</span></span>
<span data-ttu-id="cefef-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="cefef-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="cefef-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="cefef-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="cefef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cefef-130">Property</span></span>|<span data-ttu-id="cefef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cefef-131">Type</span></span>|<span data-ttu-id="cefef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cefef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cefef-133">id</span><span class="sxs-lookup"><span data-stu-id="cefef-133">id</span></span>|<span data-ttu-id="cefef-134">String</span><span class="sxs-lookup"><span data-stu-id="cefef-134">String</span></span>|<span data-ttu-id="cefef-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cefef-135">Key of the entity.</span></span> <span data-ttu-id="cefef-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cefef-137">displayName</span></span>|<span data-ttu-id="cefef-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cefef-138">String</span></span>|<span data-ttu-id="cefef-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cefef-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cefef-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-141">description</span><span class="sxs-lookup"><span data-stu-id="cefef-141">description</span></span>|<span data-ttu-id="cefef-142">String</span><span class="sxs-lookup"><span data-stu-id="cefef-142">String</span></span>|<span data-ttu-id="cefef-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cefef-143">The description of the app.</span></span> <span data-ttu-id="cefef-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-145">publicador</span><span class="sxs-lookup"><span data-stu-id="cefef-145">publisher</span></span>|<span data-ttu-id="cefef-146">String</span><span class="sxs-lookup"><span data-stu-id="cefef-146">String</span></span>|<span data-ttu-id="cefef-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cefef-147">The publisher of the app.</span></span> <span data-ttu-id="cefef-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cefef-149">largeIcon</span></span>|[<span data-ttu-id="cefef-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cefef-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cefef-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cefef-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cefef-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cefef-153">createdDateTime</span></span>|<span data-ttu-id="cefef-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cefef-154">DateTimeOffset</span></span>|<span data-ttu-id="cefef-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cefef-155">The date and time the app was created.</span></span> <span data-ttu-id="cefef-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cefef-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cefef-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cefef-158">DateTimeOffset</span></span>|<span data-ttu-id="cefef-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cefef-159">The date and time the app was last modified.</span></span> <span data-ttu-id="cefef-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cefef-161">isFeatured</span></span>|<span data-ttu-id="cefef-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefef-162">Boolean</span></span>|<span data-ttu-id="cefef-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cefef-164">privacyInformationUrl</span></span>|<span data-ttu-id="cefef-165">String</span><span class="sxs-lookup"><span data-stu-id="cefef-165">String</span></span>|<span data-ttu-id="cefef-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cefef-166">The privacy statement Url.</span></span> <span data-ttu-id="cefef-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cefef-168">informationUrl</span></span>|<span data-ttu-id="cefef-169">String</span><span class="sxs-lookup"><span data-stu-id="cefef-169">String</span></span>|<span data-ttu-id="cefef-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cefef-170">The more information Url.</span></span> <span data-ttu-id="cefef-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-172">owner</span><span class="sxs-lookup"><span data-stu-id="cefef-172">owner</span></span>|<span data-ttu-id="cefef-173">String</span><span class="sxs-lookup"><span data-stu-id="cefef-173">String</span></span>|<span data-ttu-id="cefef-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cefef-174">The owner of the app.</span></span> <span data-ttu-id="cefef-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-176">developer</span><span class="sxs-lookup"><span data-stu-id="cefef-176">developer</span></span>|<span data-ttu-id="cefef-177">String</span><span class="sxs-lookup"><span data-stu-id="cefef-177">String</span></span>|<span data-ttu-id="cefef-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cefef-178">The developer of the app.</span></span> <span data-ttu-id="cefef-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-180">notes</span><span class="sxs-lookup"><span data-stu-id="cefef-180">notes</span></span>|<span data-ttu-id="cefef-181">String</span><span class="sxs-lookup"><span data-stu-id="cefef-181">String</span></span>|<span data-ttu-id="cefef-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cefef-182">Notes for the app.</span></span> <span data-ttu-id="cefef-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="cefef-184">uploadState</span></span>|<span data-ttu-id="cefef-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cefef-185">Int32</span></span>|<span data-ttu-id="cefef-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="cefef-186">The upload state.</span></span> <span data-ttu-id="cefef-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="cefef-188">publishingState</span></span>|[<span data-ttu-id="cefef-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cefef-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cefef-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cefef-190">The publishing state for the app.</span></span> <span data-ttu-id="cefef-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cefef-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cefef-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cefef-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="cefef-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cefef-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cefef-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cefef-194">isAssigned</span></span>|<span data-ttu-id="cefef-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefef-195">Boolean</span></span>|<span data-ttu-id="cefef-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="cefef-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cefef-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cefef-198">roleScopeTagIds</span></span>|<span data-ttu-id="cefef-199">String collection</span><span class="sxs-lookup"><span data-stu-id="cefef-199">String collection</span></span>|<span data-ttu-id="cefef-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="cefef-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cefef-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="cefef-202">dependentAppCount</span></span>|<span data-ttu-id="cefef-203">Int32</span><span class="sxs-lookup"><span data-stu-id="cefef-203">Int32</span></span>|<span data-ttu-id="cefef-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="cefef-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cefef-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cefef-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cefef-206">committedContentVersion</span></span>|<span data-ttu-id="cefef-207">String</span><span class="sxs-lookup"><span data-stu-id="cefef-207">String</span></span>|<span data-ttu-id="cefef-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="cefef-208">The internal committed content version.</span></span> <span data-ttu-id="cefef-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cefef-210">fileName</span><span class="sxs-lookup"><span data-stu-id="cefef-210">fileName</span></span>|<span data-ttu-id="cefef-211">String</span><span class="sxs-lookup"><span data-stu-id="cefef-211">String</span></span>|<span data-ttu-id="cefef-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="cefef-212">The name of the main Lob application file.</span></span> <span data-ttu-id="cefef-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cefef-214">size</span><span class="sxs-lookup"><span data-stu-id="cefef-214">size</span></span>|<span data-ttu-id="cefef-215">Int64</span><span class="sxs-lookup"><span data-stu-id="cefef-215">Int64</span></span>|<span data-ttu-id="cefef-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="cefef-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="cefef-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cefef-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="cefef-218">applicableArchitectures</span></span>|[<span data-ttu-id="cefef-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="cefef-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="cefef-220">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="cefef-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="cefef-221">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="cefef-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="cefef-222">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="cefef-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="cefef-223">identityName</span><span class="sxs-lookup"><span data-stu-id="cefef-223">identityName</span></span>|<span data-ttu-id="cefef-224">String</span><span class="sxs-lookup"><span data-stu-id="cefef-224">String</span></span>|<span data-ttu-id="cefef-225">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="cefef-225">The Identity Name.</span></span> <span data-ttu-id="cefef-226">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cefef-227">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="cefef-227">identityPublisherHash</span></span>|<span data-ttu-id="cefef-228">String</span><span class="sxs-lookup"><span data-stu-id="cefef-228">String</span></span>|<span data-ttu-id="cefef-229">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="cefef-229">The Identity Publisher Hash.</span></span> <span data-ttu-id="cefef-230">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cefef-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cefef-231">identityResourceIdentifier</span></span>|<span data-ttu-id="cefef-232">String</span><span class="sxs-lookup"><span data-stu-id="cefef-232">String</span></span>|<span data-ttu-id="cefef-233">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="cefef-233">The Identity Resource Identifier.</span></span> <span data-ttu-id="cefef-234">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cefef-235">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cefef-235">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cefef-236">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cefef-236">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="cefef-237">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="cefef-237">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="cefef-238">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cefef-239">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="cefef-239">phoneProductIdentifier</span></span>|<span data-ttu-id="cefef-240">String</span><span class="sxs-lookup"><span data-stu-id="cefef-240">String</span></span>|<span data-ttu-id="cefef-241">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="cefef-241">The Phone Product Identifier.</span></span> <span data-ttu-id="cefef-242">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-242">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cefef-243">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="cefef-243">phonePublisherId</span></span>|<span data-ttu-id="cefef-244">String</span><span class="sxs-lookup"><span data-stu-id="cefef-244">String</span></span>|<span data-ttu-id="cefef-245">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-245">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cefef-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cefef-246">identityVersion</span></span>|<span data-ttu-id="cefef-247">String</span><span class="sxs-lookup"><span data-stu-id="cefef-247">String</span></span>|<span data-ttu-id="cefef-248">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="cefef-248">The identity version.</span></span> <span data-ttu-id="cefef-249">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-249">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cefef-250">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="cefef-250">appXPackageInformationList</span></span>|<span data-ttu-id="cefef-251">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="cefef-251">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="cefef-252">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="cefef-252">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="cefef-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="cefef-253">Response</span></span>
<span data-ttu-id="cefef-254">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cefef-254">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cefef-255">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cefef-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="cefef-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cefef-256">Request</span></span>
<span data-ttu-id="cefef-257">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cefef-257">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cefef-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="cefef-258">Response</span></span>
<span data-ttu-id="cefef-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cefef-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





