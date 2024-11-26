# Teste Técnico EVT

Modelagem de dados em XML e JSON para um exemplo de produtos de um laboratório com objetivo de demonstrar o entendimento sobre diferentes formatos de payload e como representá-los.

## Estruturas de Dados

### Formato JSON
```json
{
  "Paciente": {
    "id": "123",
    "nome": "João Pedro",
    "dataNascimento": "2001-12-10",
    "sexo": "masculino",
    "telefone": "(11) 98765-4321",
    "email": "joao.pedro@email.com",
    "convenio": {
      "id": "678",
      "nome": "SulAmerica",
      "dataInicio": "2023-01-01",
      "dataFim": "2024-01-01"
    }
  },
  "Consulta": {
    "id": "456",
    "pacienteId": "123",
    "medicoId": "111",
    "dataConsulta": "2023-12-01T14:30:00",
    "especialidade": "Cardiologia",
    "status": "Agendada",
    "observacoes": "Paciente relatou dores no peito.",
    "dataRegistro": "2023-11-25T15:00:00"
  }
}
```

### XML

```xml
<Paciente>
  <id>123</id>
  <nome>João Pedro</nome>
  <dataNascimento>2001-12-10</dataNascimento>
  <sexo>masculino</sexo>
  <telefone>(11) 98765-4321</telefone>
  <email>joao.pedro@email.com</email>
  <convenio>
    <id>678</id>
    <nome>SulAmerica</nome>
    <dataInicio>2023-01-01</dataInicio>
    <dataFim>2024-01-01</dataFim>
  </convenio>
</Paciente>
<Consulta>
  <id>456</id>
  <pacienteId>123</pacienteId>
  <medicoId>111</medicoId>
  <dataConsulta>2023-12-01T14:30:00</dataConsulta>
  <especialidade>Cardiologia</especialidade>
  <status>Agendada</status>
  <observacoes>Paciente relatou dores no peito.</observacoes>
  <dataRegistro>2023-11-25T15:00:00</dataRegistro>
</Consulta>
```
