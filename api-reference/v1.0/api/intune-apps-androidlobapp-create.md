---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: tfitzmac
ms.openlocfilehash: 6c0840b1da223effddd8f22687539e6f7258521b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309650"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="d3c0d-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="d3c0d-103">Create androidLobApp</span></span>

> <span data-ttu-id="d3c0d-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3c0d-105">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3c0d-105">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3c0d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3c0d-106">Prerequisites</span></span>
<span data-ttu-id="d3c0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3c0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c0d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3c0d-109">Permission type</span></span>|<span data-ttu-id="d3c0d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3c0d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3c0d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c0d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3c0d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3c0d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-114">Not supported.</span></span>|
|<span data-ttu-id="d3c0d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3c0d-115">Application</span></span>|<span data-ttu-id="d3c0d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3c0d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3c0d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d3c0d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c0d-118">Request headers</span></span>
|<span data-ttu-id="d3c0d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3c0d-119">Header</span></span>|<span data-ttu-id="d3c0d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d3c0d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3c0d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3c0d-121">Authorization</span></span>|<span data-ttu-id="d3c0d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3c0d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d3c0d-123">Accept</span></span>|<span data-ttu-id="d3c0d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3c0d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3c0d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c0d-125">Request body</span></span>
<span data-ttu-id="d3c0d-126">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-126">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="d3c0d-127">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-127">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="d3c0d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3c0d-128">Property</span></span>|<span data-ttu-id="d3c0d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3c0d-129">Type</span></span>|<span data-ttu-id="d3c0d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3c0d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c0d-131">id</span><span class="sxs-lookup"><span data-stu-id="d3c0d-131">id</span></span>|<span data-ttu-id="d3c0d-132">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-132">String</span></span>|<span data-ttu-id="d3c0d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-133">Key of the entity.</span></span> <span data-ttu-id="d3c0d-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d3c0d-135">displayName</span></span>|<span data-ttu-id="d3c0d-136">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-136">String</span></span>|<span data-ttu-id="d3c0d-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d3c0d-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-139">description</span><span class="sxs-lookup"><span data-stu-id="d3c0d-139">description</span></span>|<span data-ttu-id="d3c0d-140">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-140">String</span></span>|<span data-ttu-id="d3c0d-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-141">The description of the app.</span></span> <span data-ttu-id="d3c0d-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="d3c0d-143">publisher</span></span>|<span data-ttu-id="d3c0d-144">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-144">String</span></span>|<span data-ttu-id="d3c0d-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-145">The publisher of the app.</span></span> <span data-ttu-id="d3c0d-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d3c0d-147">largeIcon</span></span>|[<span data-ttu-id="d3c0d-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d3c0d-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d3c0d-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d3c0d-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3c0d-151">createdDateTime</span></span>|<span data-ttu-id="d3c0d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3c0d-152">DateTimeOffset</span></span>|<span data-ttu-id="d3c0d-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-153">The date and time the app was created.</span></span> <span data-ttu-id="d3c0d-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3c0d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d3c0d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3c0d-156">DateTimeOffset</span></span>|<span data-ttu-id="d3c0d-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-157">The date and time the app was last modified.</span></span> <span data-ttu-id="d3c0d-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d3c0d-159">isFeatured</span></span>|<span data-ttu-id="d3c0d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3c0d-160">Boolean</span></span>|<span data-ttu-id="d3c0d-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d3c0d-162">privacyInformationUrl</span></span>|<span data-ttu-id="d3c0d-163">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-163">String</span></span>|<span data-ttu-id="d3c0d-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-164">The privacy statement Url.</span></span> <span data-ttu-id="d3c0d-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d3c0d-166">informationUrl</span></span>|<span data-ttu-id="d3c0d-167">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-167">String</span></span>|<span data-ttu-id="d3c0d-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-168">The more information Url.</span></span> <span data-ttu-id="d3c0d-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-170">owner</span><span class="sxs-lookup"><span data-stu-id="d3c0d-170">owner</span></span>|<span data-ttu-id="d3c0d-171">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-171">String</span></span>|<span data-ttu-id="d3c0d-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-172">The owner of the app.</span></span> <span data-ttu-id="d3c0d-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-174">developer</span><span class="sxs-lookup"><span data-stu-id="d3c0d-174">developer</span></span>|<span data-ttu-id="d3c0d-175">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-175">String</span></span>|<span data-ttu-id="d3c0d-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-176">The developer of the app.</span></span> <span data-ttu-id="d3c0d-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-178">Observações</span><span class="sxs-lookup"><span data-stu-id="d3c0d-178">notes</span></span>|<span data-ttu-id="d3c0d-179">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-179">String</span></span>|<span data-ttu-id="d3c0d-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-180">Notes for the app.</span></span> <span data-ttu-id="d3c0d-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c0d-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="d3c0d-182">publishingState</span></span>|[<span data-ttu-id="d3c0d-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d3c0d-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d3c0d-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-184">The publishing state for the app.</span></span> <span data-ttu-id="d3c0d-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d3c0d-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3c0d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d3c0d-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d3c0d-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d3c0d-188">committedContentVersion</span></span>|<span data-ttu-id="d3c0d-189">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-189">String</span></span>|<span data-ttu-id="d3c0d-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-190">The internal committed content version.</span></span> <span data-ttu-id="d3c0d-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d3c0d-192">fileName</span><span class="sxs-lookup"><span data-stu-id="d3c0d-192">fileName</span></span>|<span data-ttu-id="d3c0d-193">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-193">String</span></span>|<span data-ttu-id="d3c0d-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-194">The name of the main Lob application file.</span></span> <span data-ttu-id="d3c0d-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d3c0d-196">size</span><span class="sxs-lookup"><span data-stu-id="d3c0d-196">size</span></span>|<span data-ttu-id="d3c0d-197">Int64</span><span class="sxs-lookup"><span data-stu-id="d3c0d-197">Int64</span></span>|<span data-ttu-id="d3c0d-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="d3c0d-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c0d-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d3c0d-200">packageId</span><span class="sxs-lookup"><span data-stu-id="d3c0d-200">packageId</span></span>|<span data-ttu-id="d3c0d-201">String</span><span class="sxs-lookup"><span data-stu-id="d3c0d-201">String</span></span>|<span data-ttu-id="d3c0d-202">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-202">The package identifier.</span></span>|
|<span data-ttu-id="d3c0d-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d3c0d-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d3c0d-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d3c0d-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="d3c0d-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d3c0d-206">versionName</span><span class="sxs-lookup"><span data-stu-id="d3c0d-206">versionName</span></span>|<span data-ttu-id="d3c0d-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3c0d-207">String</span></span>|<span data-ttu-id="d3c0d-208">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d3c0d-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="d3c0d-209">versionCode</span></span>|<span data-ttu-id="d3c0d-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3c0d-210">String</span></span>|<span data-ttu-id="d3c0d-211">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="d3c0d-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3c0d-212">Response</span></span>
<span data-ttu-id="d3c0d-213">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-213">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3c0d-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3c0d-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3c0d-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c0d-215">Request</span></span>
<span data-ttu-id="d3c0d-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1075

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="d3c0d-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3c0d-217">Response</span></span>
<span data-ttu-id="d3c0d-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3c0d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



