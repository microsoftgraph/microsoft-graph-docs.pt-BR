# <a name="reportroot-getonedriveusageaccountcounts"></a>reportRoot: getOneDriveUsageAccountCounts

Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :--------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                           |
| Aplicativo                            | Reports.Read.All                         |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="request-parameters"></a>Solicitar parâmetros

Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | string | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: D7, D30, D90 e D180. Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado. Obrigatório. |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                              |
| :------------ | :--------------------------------------- |
| Autorização | {token} de portador. Obrigatório.                |
| If-None-Match | Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido. Opcional. |

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório. Essa URL pode ser encontrada no cabeçalho `Location` na resposta.

As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.

O arquivo CSV possui os seguintes cabeçalhos para colunas.

- Data de atualização do relatório
- Tipo de site
- Total
- Ativo
- Data do relatório
- Período de Relatório

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
