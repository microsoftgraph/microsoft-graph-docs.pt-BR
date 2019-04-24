---
title: Criar windowsMobileMSI
description: Cria um novo objeto windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5a62f94d5c15adc8ad3080109a8d45fd1f03603
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32487942"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="19fc4-103">Criar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="19fc4-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="19fc4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19fc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19fc4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19fc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19fc4-106">Cria um novo objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="19fc4-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19fc4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19fc4-107">Prerequisites</span></span>
<span data-ttu-id="19fc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19fc4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19fc4-110">Permission type</span></span>|<span data-ttu-id="19fc4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19fc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19fc4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19fc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19fc4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fc4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19fc4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19fc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19fc4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19fc4-115">Not supported.</span></span>|
|<span data-ttu-id="19fc4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19fc4-116">Application</span></span>|<span data-ttu-id="19fc4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19fc4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19fc4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19fc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="19fc4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19fc4-119">Request headers</span></span>
|<span data-ttu-id="19fc4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19fc4-120">Header</span></span>|<span data-ttu-id="19fc4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="19fc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19fc4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="19fc4-122">Authorization</span></span>|<span data-ttu-id="19fc4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19fc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19fc4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19fc4-124">Accept</span></span>|<span data-ttu-id="19fc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19fc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19fc4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19fc4-126">Request body</span></span>
<span data-ttu-id="19fc4-127">No corpo da solicitação, forneça uma representação JSON para o objeto windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="19fc4-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="19fc4-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="19fc4-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="19fc4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19fc4-129">Property</span></span>|<span data-ttu-id="19fc4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="19fc4-130">Type</span></span>|<span data-ttu-id="19fc4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="19fc4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19fc4-132">id</span><span class="sxs-lookup"><span data-stu-id="19fc4-132">id</span></span>|<span data-ttu-id="19fc4-133">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-133">String</span></span>|<span data-ttu-id="19fc4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="19fc4-134">Key of the entity.</span></span> <span data-ttu-id="19fc4-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="19fc4-136">displayName</span></span>|<span data-ttu-id="19fc4-137">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-137">String</span></span>|<span data-ttu-id="19fc4-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="19fc4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="19fc4-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-140">description</span><span class="sxs-lookup"><span data-stu-id="19fc4-140">description</span></span>|<span data-ttu-id="19fc4-141">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-141">String</span></span>|<span data-ttu-id="19fc4-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-142">The description of the app.</span></span> <span data-ttu-id="19fc4-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-144">publicador</span><span class="sxs-lookup"><span data-stu-id="19fc4-144">publisher</span></span>|<span data-ttu-id="19fc4-145">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-145">String</span></span>|<span data-ttu-id="19fc4-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-146">The publisher of the app.</span></span> <span data-ttu-id="19fc4-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="19fc4-148">largeIcon</span></span>|[<span data-ttu-id="19fc4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="19fc4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="19fc4-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="19fc4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="19fc4-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19fc4-152">createdDateTime</span></span>|<span data-ttu-id="19fc4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19fc4-153">DateTimeOffset</span></span>|<span data-ttu-id="19fc4-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-154">The date and time the app was created.</span></span> <span data-ttu-id="19fc4-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19fc4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="19fc4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19fc4-157">DateTimeOffset</span></span>|<span data-ttu-id="19fc4-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="19fc4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="19fc4-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="19fc4-160">isFeatured</span></span>|<span data-ttu-id="19fc4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="19fc4-161">Boolean</span></span>|<span data-ttu-id="19fc4-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="19fc4-163">privacyInformationUrl</span></span>|<span data-ttu-id="19fc4-164">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-164">String</span></span>|<span data-ttu-id="19fc4-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="19fc4-165">The privacy statement Url.</span></span> <span data-ttu-id="19fc4-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="19fc4-167">informationUrl</span></span>|<span data-ttu-id="19fc4-168">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-168">String</span></span>|<span data-ttu-id="19fc4-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="19fc4-169">The more information Url.</span></span> <span data-ttu-id="19fc4-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-171">owner</span><span class="sxs-lookup"><span data-stu-id="19fc4-171">owner</span></span>|<span data-ttu-id="19fc4-172">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-172">String</span></span>|<span data-ttu-id="19fc4-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-173">The owner of the app.</span></span> <span data-ttu-id="19fc4-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-175">developer</span><span class="sxs-lookup"><span data-stu-id="19fc4-175">developer</span></span>|<span data-ttu-id="19fc4-176">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-176">String</span></span>|<span data-ttu-id="19fc4-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-177">The developer of the app.</span></span> <span data-ttu-id="19fc4-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-179">notes</span><span class="sxs-lookup"><span data-stu-id="19fc4-179">notes</span></span>|<span data-ttu-id="19fc4-180">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-180">String</span></span>|<span data-ttu-id="19fc4-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-181">Notes for the app.</span></span> <span data-ttu-id="19fc4-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="19fc4-183">uploadState</span></span>|<span data-ttu-id="19fc4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="19fc4-184">Int32</span></span>|<span data-ttu-id="19fc4-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="19fc4-185">The upload state.</span></span> <span data-ttu-id="19fc4-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="19fc4-187">publishingState</span></span>|[<span data-ttu-id="19fc4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="19fc4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="19fc4-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-189">The publishing state for the app.</span></span> <span data-ttu-id="19fc4-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="19fc4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="19fc4-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19fc4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="19fc4-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="19fc4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="19fc4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="19fc4-193">isAssigned</span></span>|<span data-ttu-id="19fc4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="19fc4-194">Boolean</span></span>|<span data-ttu-id="19fc4-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="19fc4-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19fc4-197">roleScopeTagIds</span></span>|<span data-ttu-id="19fc4-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="19fc4-198">String collection</span></span>|<span data-ttu-id="19fc4-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="19fc4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="19fc4-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="19fc4-201">dependentAppCount</span></span>|<span data-ttu-id="19fc4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="19fc4-202">Int32</span></span>|<span data-ttu-id="19fc4-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="19fc4-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="19fc4-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19fc4-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="19fc4-205">committedContentVersion</span></span>|<span data-ttu-id="19fc4-206">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-206">String</span></span>|<span data-ttu-id="19fc4-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="19fc4-207">The internal committed content version.</span></span> <span data-ttu-id="19fc4-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="19fc4-209">fileName</span><span class="sxs-lookup"><span data-stu-id="19fc4-209">fileName</span></span>|<span data-ttu-id="19fc4-210">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-210">String</span></span>|<span data-ttu-id="19fc4-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="19fc4-211">The name of the main Lob application file.</span></span> <span data-ttu-id="19fc4-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="19fc4-213">size</span><span class="sxs-lookup"><span data-stu-id="19fc4-213">size</span></span>|<span data-ttu-id="19fc4-214">Int64</span><span class="sxs-lookup"><span data-stu-id="19fc4-214">Int64</span></span>|<span data-ttu-id="19fc4-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="19fc4-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="19fc4-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="19fc4-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="19fc4-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="19fc4-217">commandLine</span></span>|<span data-ttu-id="19fc4-218">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-218">String</span></span>|<span data-ttu-id="19fc4-219">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="19fc4-219">The command line.</span></span>|
|<span data-ttu-id="19fc4-220">productCode</span><span class="sxs-lookup"><span data-stu-id="19fc4-220">productCode</span></span>|<span data-ttu-id="19fc4-221">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-221">String</span></span>|<span data-ttu-id="19fc4-222">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="19fc4-222">The product code.</span></span>|
|<span data-ttu-id="19fc4-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="19fc4-223">productVersion</span></span>|<span data-ttu-id="19fc4-224">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-224">String</span></span>|<span data-ttu-id="19fc4-225">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="19fc4-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="19fc4-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="19fc4-226">ignoreVersionDetection</span></span>|<span data-ttu-id="19fc4-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="19fc4-227">Boolean</span></span>|<span data-ttu-id="19fc4-228">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="19fc4-229">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="19fc4-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="19fc4-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="19fc4-230">identityVersion</span></span>|<span data-ttu-id="19fc4-231">String</span><span class="sxs-lookup"><span data-stu-id="19fc4-231">String</span></span>|<span data-ttu-id="19fc4-232">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="19fc4-232">The identity version.</span></span>|
|<span data-ttu-id="19fc4-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="19fc4-233">useDeviceContext</span></span>|<span data-ttu-id="19fc4-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="19fc4-234">Boolean</span></span>|<span data-ttu-id="19fc4-235">Indica se um MSI de modo duplo deve ser instalado no contexto de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="19fc4-236">Se true, o aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="19fc4-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="19fc4-237">Se false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="19fc4-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="19fc4-238">Se for NULL, o serviço usará o contexto de instalação padrão do pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="19fc4-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="19fc4-239">No caso do MSI de modo duplo, esse padrão será por usuário.</span><span class="sxs-lookup"><span data-stu-id="19fc4-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="19fc4-240">Não pode ser definido para aplicativos de modo não duplo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="19fc4-241">Não pode ser alterado após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19fc4-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="19fc4-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="19fc4-242">Response</span></span>
<span data-ttu-id="19fc4-243">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19fc4-243">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19fc4-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19fc4-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="19fc4-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19fc4-245">Request</span></span>
<span data-ttu-id="19fc4-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19fc4-246">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19fc4-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="19fc4-247">Response</span></span>
<span data-ttu-id="19fc4-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19fc4-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





