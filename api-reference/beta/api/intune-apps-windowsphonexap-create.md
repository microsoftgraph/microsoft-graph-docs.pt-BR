---
title: Criar windowsPhoneXAP
description: Crie um novo objeto de windowsPhoneXAP.
ms.openlocfilehash: 8b22ed8d9294c8e7a3e5c2e91e5b3d82e8f6bce9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040261"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="ea63d-103">Criar windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="ea63d-103">Create windowsPhoneXAP</span></span>

> <span data-ttu-id="ea63d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea63d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea63d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea63d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea63d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea63d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea63d-107">Crie um novo objeto de [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="ea63d-107">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea63d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea63d-108">Prerequisites</span></span>
<span data-ttu-id="ea63d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea63d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea63d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea63d-111">Permission type</span></span>|<span data-ttu-id="ea63d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea63d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea63d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea63d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea63d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea63d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea63d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea63d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea63d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea63d-116">Not supported.</span></span>|
|<span data-ttu-id="ea63d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea63d-117">Application</span></span>|<span data-ttu-id="ea63d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea63d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea63d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea63d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ea63d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea63d-120">Request headers</span></span>
|<span data-ttu-id="ea63d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea63d-121">Header</span></span>|<span data-ttu-id="ea63d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ea63d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea63d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea63d-123">Authorization</span></span>|<span data-ttu-id="ea63d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea63d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea63d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea63d-125">Accept</span></span>|<span data-ttu-id="ea63d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea63d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea63d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea63d-127">Request body</span></span>
<span data-ttu-id="ea63d-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhoneXAP.</span><span class="sxs-lookup"><span data-stu-id="ea63d-128">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="ea63d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhoneXAP.</span><span class="sxs-lookup"><span data-stu-id="ea63d-129">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="ea63d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea63d-130">Property</span></span>|<span data-ttu-id="ea63d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea63d-131">Type</span></span>|<span data-ttu-id="ea63d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea63d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea63d-133">id</span><span class="sxs-lookup"><span data-stu-id="ea63d-133">id</span></span>|<span data-ttu-id="ea63d-134">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-134">String</span></span>|<span data-ttu-id="ea63d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea63d-135">Key of the entity.</span></span> <span data-ttu-id="ea63d-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ea63d-137">displayName</span></span>|<span data-ttu-id="ea63d-138">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-138">String</span></span>|<span data-ttu-id="ea63d-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ea63d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ea63d-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-141">description</span><span class="sxs-lookup"><span data-stu-id="ea63d-141">description</span></span>|<span data-ttu-id="ea63d-142">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-142">String</span></span>|<span data-ttu-id="ea63d-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea63d-143">The description of the app.</span></span> <span data-ttu-id="ea63d-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ea63d-145">publisher</span></span>|<span data-ttu-id="ea63d-146">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-146">String</span></span>|<span data-ttu-id="ea63d-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea63d-147">The publisher of the app.</span></span> <span data-ttu-id="ea63d-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ea63d-149">largeIcon</span></span>|[<span data-ttu-id="ea63d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ea63d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ea63d-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ea63d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ea63d-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea63d-153">createdDateTime</span></span>|<span data-ttu-id="ea63d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea63d-154">DateTimeOffset</span></span>|<span data-ttu-id="ea63d-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea63d-155">The date and time the app was created.</span></span> <span data-ttu-id="ea63d-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea63d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ea63d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea63d-158">DateTimeOffset</span></span>|<span data-ttu-id="ea63d-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ea63d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ea63d-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ea63d-161">isFeatured</span></span>|<span data-ttu-id="ea63d-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="ea63d-162">Boolean</span></span>|<span data-ttu-id="ea63d-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ea63d-164">privacyInformationUrl</span></span>|<span data-ttu-id="ea63d-165">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-165">String</span></span>|<span data-ttu-id="ea63d-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ea63d-166">The privacy statement Url.</span></span> <span data-ttu-id="ea63d-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ea63d-168">informationUrl</span></span>|<span data-ttu-id="ea63d-169">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-169">String</span></span>|<span data-ttu-id="ea63d-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ea63d-170">The more information Url.</span></span> <span data-ttu-id="ea63d-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-172">owner</span><span class="sxs-lookup"><span data-stu-id="ea63d-172">owner</span></span>|<span data-ttu-id="ea63d-173">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-173">String</span></span>|<span data-ttu-id="ea63d-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ea63d-174">The owner of the app.</span></span> <span data-ttu-id="ea63d-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-176">developer</span><span class="sxs-lookup"><span data-stu-id="ea63d-176">developer</span></span>|<span data-ttu-id="ea63d-177">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-177">String</span></span>|<span data-ttu-id="ea63d-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea63d-178">The developer of the app.</span></span> <span data-ttu-id="ea63d-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-180">Observações</span><span class="sxs-lookup"><span data-stu-id="ea63d-180">notes</span></span>|<span data-ttu-id="ea63d-181">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-181">String</span></span>|<span data-ttu-id="ea63d-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea63d-182">Notes for the app.</span></span> <span data-ttu-id="ea63d-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ea63d-184">uploadState</span></span>|<span data-ttu-id="ea63d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ea63d-185">Int32</span></span>|<span data-ttu-id="ea63d-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="ea63d-186">The upload state.</span></span> <span data-ttu-id="ea63d-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea63d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ea63d-188">publishingState</span></span>|[<span data-ttu-id="ea63d-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ea63d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ea63d-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea63d-190">The publishing state for the app.</span></span> <span data-ttu-id="ea63d-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ea63d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ea63d-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ea63d-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ea63d-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ea63d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ea63d-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ea63d-194">committedContentVersion</span></span>|<span data-ttu-id="ea63d-195">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-195">String</span></span>|<span data-ttu-id="ea63d-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ea63d-196">The internal committed content version.</span></span> <span data-ttu-id="ea63d-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ea63d-198">fileName</span><span class="sxs-lookup"><span data-stu-id="ea63d-198">fileName</span></span>|<span data-ttu-id="ea63d-199">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-199">String</span></span>|<span data-ttu-id="ea63d-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ea63d-200">The name of the main Lob application file.</span></span> <span data-ttu-id="ea63d-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ea63d-202">size</span><span class="sxs-lookup"><span data-stu-id="ea63d-202">size</span></span>|<span data-ttu-id="ea63d-203">Int64</span><span class="sxs-lookup"><span data-stu-id="ea63d-203">Int64</span></span>|<span data-ttu-id="ea63d-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ea63d-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="ea63d-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea63d-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ea63d-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ea63d-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ea63d-207">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ea63d-207">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ea63d-208">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ea63d-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ea63d-209">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="ea63d-209">productIdentifier</span></span>|<span data-ttu-id="ea63d-210">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-210">String</span></span>|<span data-ttu-id="ea63d-211">O identificador do produto.</span><span class="sxs-lookup"><span data-stu-id="ea63d-211">The Product Identifier.</span></span>|
|<span data-ttu-id="ea63d-212">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ea63d-212">identityVersion</span></span>|<span data-ttu-id="ea63d-213">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-213">String</span></span>|<span data-ttu-id="ea63d-214">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="ea63d-214">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ea63d-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea63d-215">Response</span></span>
<span data-ttu-id="ea63d-216">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea63d-216">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea63d-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea63d-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea63d-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea63d-218">Request</span></span>
<span data-ttu-id="ea63d-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea63d-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1143

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ea63d-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea63d-220">Response</span></span>
<span data-ttu-id="ea63d-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea63d-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





