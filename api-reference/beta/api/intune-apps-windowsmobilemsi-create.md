---
title: Criar windowsMobileMSI
description: Cria um novo objeto windowsMobileMSI.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c7f70734e9fd2805a4f84bf27e71a99955d46d3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973184"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="5d03a-103">Criar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="5d03a-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="5d03a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5d03a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d03a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d03a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d03a-106">Cria um novo objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="5d03a-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d03a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d03a-107">Prerequisites</span></span>
<span data-ttu-id="5d03a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d03a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d03a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d03a-110">Permission type</span></span>|<span data-ttu-id="5d03a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5d03a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d03a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d03a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d03a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d03a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d03a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d03a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d03a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d03a-115">Not supported.</span></span>|
|<span data-ttu-id="5d03a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d03a-116">Application</span></span>|<span data-ttu-id="5d03a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d03a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d03a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d03a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5d03a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d03a-119">Request headers</span></span>
|<span data-ttu-id="5d03a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d03a-120">Header</span></span>|<span data-ttu-id="5d03a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5d03a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d03a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d03a-122">Authorization</span></span>|<span data-ttu-id="5d03a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d03a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d03a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d03a-124">Accept</span></span>|<span data-ttu-id="5d03a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d03a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d03a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d03a-126">Request body</span></span>
<span data-ttu-id="5d03a-127">No corpo da solicitação, forneça uma representação JSON para o objeto windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="5d03a-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="5d03a-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="5d03a-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="5d03a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d03a-129">Property</span></span>|<span data-ttu-id="5d03a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d03a-130">Type</span></span>|<span data-ttu-id="5d03a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d03a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d03a-132">id</span><span class="sxs-lookup"><span data-stu-id="5d03a-132">id</span></span>|<span data-ttu-id="5d03a-133">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-133">String</span></span>|<span data-ttu-id="5d03a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5d03a-134">Key of the entity.</span></span> <span data-ttu-id="5d03a-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5d03a-136">displayName</span></span>|<span data-ttu-id="5d03a-137">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-137">String</span></span>|<span data-ttu-id="5d03a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="5d03a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5d03a-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-140">descrição</span><span class="sxs-lookup"><span data-stu-id="5d03a-140">description</span></span>|<span data-ttu-id="5d03a-141">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-141">String</span></span>|<span data-ttu-id="5d03a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-142">The description of the app.</span></span> <span data-ttu-id="5d03a-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-144">publicador</span><span class="sxs-lookup"><span data-stu-id="5d03a-144">publisher</span></span>|<span data-ttu-id="5d03a-145">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-145">String</span></span>|<span data-ttu-id="5d03a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-146">The publisher of the app.</span></span> <span data-ttu-id="5d03a-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5d03a-148">largeIcon</span></span>|[<span data-ttu-id="5d03a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d03a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5d03a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="5d03a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5d03a-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d03a-152">createdDateTime</span></span>|<span data-ttu-id="5d03a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d03a-153">DateTimeOffset</span></span>|<span data-ttu-id="5d03a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-154">The date and time the app was created.</span></span> <span data-ttu-id="5d03a-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d03a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5d03a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d03a-157">DateTimeOffset</span></span>|<span data-ttu-id="5d03a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5d03a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5d03a-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5d03a-160">isFeatured</span></span>|<span data-ttu-id="5d03a-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d03a-161">Boolean</span></span>|<span data-ttu-id="5d03a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5d03a-163">privacyInformationUrl</span></span>|<span data-ttu-id="5d03a-164">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-164">String</span></span>|<span data-ttu-id="5d03a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5d03a-165">The privacy statement Url.</span></span> <span data-ttu-id="5d03a-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5d03a-167">informationUrl</span></span>|<span data-ttu-id="5d03a-168">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-168">String</span></span>|<span data-ttu-id="5d03a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5d03a-169">The more information Url.</span></span> <span data-ttu-id="5d03a-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-171">owner</span><span class="sxs-lookup"><span data-stu-id="5d03a-171">owner</span></span>|<span data-ttu-id="5d03a-172">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-172">String</span></span>|<span data-ttu-id="5d03a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-173">The owner of the app.</span></span> <span data-ttu-id="5d03a-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-175">developer</span><span class="sxs-lookup"><span data-stu-id="5d03a-175">developer</span></span>|<span data-ttu-id="5d03a-176">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-176">String</span></span>|<span data-ttu-id="5d03a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-177">The developer of the app.</span></span> <span data-ttu-id="5d03a-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-179">notes</span><span class="sxs-lookup"><span data-stu-id="5d03a-179">notes</span></span>|<span data-ttu-id="5d03a-180">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-180">String</span></span>|<span data-ttu-id="5d03a-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-181">Notes for the app.</span></span> <span data-ttu-id="5d03a-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="5d03a-183">uploadState</span></span>|<span data-ttu-id="5d03a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5d03a-184">Int32</span></span>|<span data-ttu-id="5d03a-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="5d03a-185">The upload state.</span></span> <span data-ttu-id="5d03a-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="5d03a-187">publishingState</span></span>|[<span data-ttu-id="5d03a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5d03a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5d03a-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-189">The publishing state for the app.</span></span> <span data-ttu-id="5d03a-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="5d03a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5d03a-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d03a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5d03a-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5d03a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5d03a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5d03a-193">isAssigned</span></span>|<span data-ttu-id="5d03a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d03a-194">Boolean</span></span>|<span data-ttu-id="5d03a-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5d03a-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5d03a-197">roleScopeTagIds</span></span>|<span data-ttu-id="5d03a-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d03a-198">String collection</span></span>|<span data-ttu-id="5d03a-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="5d03a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5d03a-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="5d03a-201">dependentAppCount</span></span>|<span data-ttu-id="5d03a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="5d03a-202">Int32</span></span>|<span data-ttu-id="5d03a-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="5d03a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5d03a-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d03a-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5d03a-205">committedContentVersion</span></span>|<span data-ttu-id="5d03a-206">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-206">String</span></span>|<span data-ttu-id="5d03a-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="5d03a-207">The internal committed content version.</span></span> <span data-ttu-id="5d03a-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5d03a-209">fileName</span><span class="sxs-lookup"><span data-stu-id="5d03a-209">fileName</span></span>|<span data-ttu-id="5d03a-210">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-210">String</span></span>|<span data-ttu-id="5d03a-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="5d03a-211">The name of the main Lob application file.</span></span> <span data-ttu-id="5d03a-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5d03a-213">size</span><span class="sxs-lookup"><span data-stu-id="5d03a-213">size</span></span>|<span data-ttu-id="5d03a-214">Int64</span><span class="sxs-lookup"><span data-stu-id="5d03a-214">Int64</span></span>|<span data-ttu-id="5d03a-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="5d03a-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="5d03a-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d03a-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5d03a-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="5d03a-217">commandLine</span></span>|<span data-ttu-id="5d03a-218">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-218">String</span></span>|<span data-ttu-id="5d03a-219">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="5d03a-219">The command line.</span></span>|
|<span data-ttu-id="5d03a-220">productCode</span><span class="sxs-lookup"><span data-stu-id="5d03a-220">productCode</span></span>|<span data-ttu-id="5d03a-221">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-221">String</span></span>|<span data-ttu-id="5d03a-222">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="5d03a-222">The product code.</span></span>|
|<span data-ttu-id="5d03a-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="5d03a-223">productVersion</span></span>|<span data-ttu-id="5d03a-224">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-224">String</span></span>|<span data-ttu-id="5d03a-225">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="5d03a-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5d03a-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="5d03a-226">ignoreVersionDetection</span></span>|<span data-ttu-id="5d03a-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d03a-227">Boolean</span></span>|<span data-ttu-id="5d03a-228">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="5d03a-229">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="5d03a-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="5d03a-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5d03a-230">identityVersion</span></span>|<span data-ttu-id="5d03a-231">String</span><span class="sxs-lookup"><span data-stu-id="5d03a-231">String</span></span>|<span data-ttu-id="5d03a-232">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="5d03a-232">The identity version.</span></span>|
|<span data-ttu-id="5d03a-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="5d03a-233">useDeviceContext</span></span>|<span data-ttu-id="5d03a-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d03a-234">Boolean</span></span>|<span data-ttu-id="5d03a-235">Indica se um MSI de modo duplo deve ser instalado no contexto de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="5d03a-236">Se true, o aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="5d03a-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="5d03a-237">Se false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="5d03a-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="5d03a-238">Se for NULL, o serviço usará o contexto de instalação padrão do pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="5d03a-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="5d03a-239">No caso do MSI de modo duplo, esse padrão será por usuário.</span><span class="sxs-lookup"><span data-stu-id="5d03a-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="5d03a-240">Não pode ser definido para aplicativos de modo não duplo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="5d03a-241">Não pode ser alterado após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d03a-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="5d03a-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d03a-242">Response</span></span>
<span data-ttu-id="5d03a-243">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d03a-243">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d03a-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d03a-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d03a-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d03a-245">Request</span></span>
<span data-ttu-id="5d03a-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d03a-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="5d03a-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d03a-247">Response</span></span>
<span data-ttu-id="5d03a-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d03a-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





