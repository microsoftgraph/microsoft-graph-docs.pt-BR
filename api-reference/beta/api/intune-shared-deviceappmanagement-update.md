---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e88fca39fdd9395661bff0f0468bb54cd1b116f2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59096323"
---
# <a name="update-deviceappmanagement"></a>Atualizar deviceAppManagement

Namespace: microsoft.graph

> **Importante:** APIs na versão /beta no Microsoft Graph estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).  Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
| Delegado (conta corporativa ou de estudante) | |
| &nbsp;&nbsp; **Aplicativos,** **livros,** **integração,** **integração de** parceiros ou **conjunto de políticas** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | |
| &nbsp;&nbsp; **Aplicativos,** **livros,** **integração,** **integração de** parceiros ou **conjunto de políticas** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|**Ao abordar**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.|
|microsoftStoreForBusinessLanguage|String|As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas. Culturas específicas de um país/região. Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes). O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166. Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|As informações do portal do usuário final são usadas para sincronizar aplicativos do Microsoft Store para Empresas para Portal da Empresa do Intune. Há três opções para escolher em 'Somente portal da empresa', 'Portal da empresa e loja \[ privada', 'Somente armazenamento particular' \] . Os valores possíveis são: `none`, `companyPortal`, `privateStore`.|

Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```









